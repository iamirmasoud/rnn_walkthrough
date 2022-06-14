# Walkthrough on Recurrent Neural Networks (RNNs) in PyTorch 

## Project Overview

This repo holds the codes for a step-by-step tutorial on Recurrent Neural Networks, from Basic RNNs and complex deep LSTM networks.

---
## Preparing the environment
**Note**: I have developed this project on __Linux__. It can surely be run on Windows and Mac with some little changes.

Before you can experiment with the code, you'll have to make sure that you have all the libraries and dependencies required to support this project. You will mainly need Python 3, PyTorch and its torchvision, OpenCV, Matplotlib, and tqdm.

1. Clone the repository, and navigate to the downloaded folder.
```
git clone https://github.com/iamirmasoud/facial_keypoint_detection.git
cd facial_keypoint_detection
```

2. Create (and activate) a new environment, named `rnn_env` with Python 3.7. If prompted to proceed with the install `(Proceed [y]/n)` type y.

	```shell
	conda create -n rnn_env python=3.7
	source activate rnn_env
	```
	
	At this point your command line should look something like: `(rnn_env) <User>:facial_keypoint_detection <user>$`. The `(rnn_env)` indicates that your environment has been activated, and you can proceed with further package installations.

6. Before you can experiment with the code, you'll have to make sure that you have all the libraries and dependencies required to support this project. You will mainly need Python3.7+, PyTorch and its torchvision, OpenCV, Matplotlib. You can install  dependencies using:
```
pip install -r requirements.txt
```

7. Navigate back to the repo. (Also, your source environment should still be activated at this point.)
```shell
cd facial_keypoint_detection
```

8. Open the directory of notebooks, using the below command. You'll see all the project files appear in your local environment; open the first notebook and follow the instructions.
```shell
jupyter notebook
```

9. Once you open any of the project notebooks, make sure you are in the correct `rnn_env` environment by clicking `Kernel > Change Kernel > rnn_env`.


## Jupyter Notebooks
The project is structured as a series of Jupyter Notebooks that should be run in sequential order:

### [1_Vanilla_RNN_Basics](1_Vanilla_RNN_Basics.ipynb)

Provides the implementation of a Vanilla RNN from scratch. 

### [2_Character_Model_with_Basic_RNN](2_Character_Model_with_Basic_RNN.ipynb) 

In this notebook, I'll be implementing a simple RNN character model to familiarize ourselves with the RNNs in PyTorch library. In this implementation, I'll be building a model that can complete a sentence based on a few characters or a word used as input.


### [3_LSTM_Structure](3_LSTM_Structure.ipynb) 

In this notebook, I will introduce the basics of LSTM networks.

### [4_LSTM_Training_Part_of_Speech_Tagging](4_LSTM_Training_Part_of_Speech_Tagging.ipynb) 

In this notebook, I will use an LSTM to predict part-of-speech tags for words.

### [5_Character Level LSTM](5_Character Level LSTM.ipynb) 

In this notebook, I'll construct a character-level LSTM with PyTorch. The network will train character by character on some text, then generate new text character by character. As an example, I will train on Anna Karenina. This model will be able to generate new text based on the text from the book!


## Results

Here is a sample output from my Character-Level LSTM model trained on Anna Karenina. I got the word `"Anna"` as the starting characters.

```
Anna."

"You can be in a part of interest. I want to see you! I'm going about it," he
said. "I could not speak from you, who would be those party the side."

"Yes," said Stepan Arkadyevitch. "As you say there."

Anna said that thought of the fealing of that she had any one thing
in speating of a principle of happiness to be. In the same time, they
went up and would be at the country. He had not been a moment of signing in
the simplicity of the wearther in spotion with her. She would be in second
a moment. He considered this soul, who could both that that he had not
said, that the waiters had been perfectly carched a death in her. But the
world was a perfect angry. A choochands were carried into the money which the
partition was standing in the side of the feel. He confined the town, he
had never been so thinking of all is there and sentratuats in his
breadings, he would have said, as the same time he was there at the
sound, and he had not come, with his wife and her eyes were coming to the
chillren, and that he had studied and saw that her hand and her striggers,
work that is to be already in a passed on one of the same short impression
to the sound of that she did not take him to her. And what was still
might be better to see him that touching his hand at the same time,
when the parance, throw on the class.

"Well, while I such a musical tour about any sounder all of my silence that
had to go on in the country?"

"Oh, I could have means to do a matter to make you some time."

"Oh! I were going to bode. I'm sorry for the. I shall go and consider that
though a man who, this could be at the painter," said the old
man, that was the more from the service, who had been almost sight, and
had not to bought a cold bart. She came up. At those whom, some dinence,
to be supposed. He was sennial time to take the side. The chincess
struck her he would be sent and defend that the country, wished from her
side of his suffering and should not be a place, and so aware of the
money though
```