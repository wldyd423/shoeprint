# shoeprint
Prototype work that I may or maynot use in the future. Guided by ppt from Forensics@NIST

Original ppt
https://www.nist.gov/system/files/documents/2018/11/14/3_padi_s.pdf


Database used:

https://fid.dmi.unibas.ch/

Their paper:

https://fid.dmi.unibas.ch/FID_ACCV14.pdf



This project is a prototype project to check if using a Siamese Network for Shoe Impression Similarity Check is a valid approach.

Unfortunately it seems that more data is required. Furthermore Siamese Network detects the similrity between two inputs not classify it. It could be done by scanning through the whole reference and look for the highest accuracy value do classify the target. This however is O(N) complexity so the larger the database the slower the AI.

The reason I used Siamese Network was because I didn't really understand the ppt's method. It was ResNet50 finetuning taking two inputs, a reference and a target. Then they used a similarity metric to determine the similarity between two encoded features. This was generally similar with Siamese Network apart from the fact that Siamese seem to use euclidean distance. 

Nevertheless, I learned new things and I would love to stick with network next time. I hope