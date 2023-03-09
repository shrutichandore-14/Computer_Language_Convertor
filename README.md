# Computer_Language_Convertor


*About*

A transcoder is a type of computer software that can convert one computer language to another one. Transcoding is the process of converting digital data from one encoding format to another, which is often necessary when transferring media files between different devices or systems that use different file formats.


*Dependencies*

Python 3
NumPy
PyTorch
fastBPE (generate and apply BPE codes)
Moses (scripts to clean and tokenize text only - no installation required)
Apex (for fp16 training)
libclang (for C++ tokenization)
submitit (to run the preprocessing pipeline on remote machine)
six
sacrebleu (pip install sacrebleu=="1.2.11")


*Translate*

Transcompilation between Java, C++ and Python 3.
The model can be tested on new inputs using the translate.py script.
For instance, python translate.py --src_lang cpp --tgt_lang java --model_path trained_model.pth < input_code.cpp will translate the C++ code contained in input_code.cpp to Java.


*PreTrained Models*

 * C++ -> Java, Java -> C++ and Java -> Python
 * C++ -> Python, Python -> C++ and Python -> Java
