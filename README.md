# custom_dsw_transformer
Custom Dilated Sliding Window Attention Transformer in Tensorflow

Before the advent of large language models with 100,000 + token context windows I was interested in the mathematical underpinnings that hindered transformer-based models from 'ingesting' long documents. At the time chunking was the only viable option, but if I settled on chunking I would lose information quality because the attention mechanism would not be computed across the entire document. It would only be computed across the various chunks, and then I'd have to average the attention scores...not ideal.

This was my attempt at implementing a Dilated Sliding Window Attention, and guiding the output using an algorithm I developed for my master's thesis in 2023. 

The inspiration for the code comes from, "Longformer: The Long-Document Transformer" Iz Beltagy, Matthew E. Peters, and Arman Cohan from the Allen Institute for Artificial Intelligence, April 2020.
![DilatedSlidingWindow](https://github.com/user-attachments/assets/dc55ee96-8c7b-4f39-aa02-bed290b9672f)
