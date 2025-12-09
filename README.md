# base119
Processing Base Blockchain Blocks Sequentially  Useful for indexing.  Python example
start = w3.eth.block_number - 50
for b in range(start, start+50):
    block = w3.eth.get_block(b)
    print(b, len(block.transactions))
