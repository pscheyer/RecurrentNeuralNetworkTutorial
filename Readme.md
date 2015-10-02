20151001 1842CST
#Recurrent Neural Network Tutorial

This is a clone of [DennyBritz's RNN Tutorial](https://github.com/dennybritz/rnn-tutorial-rnnlm) described in detail in the [associated blog post](http://www.wildml.com/2015/09/recurrent-neural-networks-tutorial-part-2-implementing-a-language-model-rnn-with-python-numpy-and-theano/)
I am also using it as an opportunity to learn `virtualenv` for running python apps in containers. 

I already ran
```bash
$ sudo pip install virtualenv
```
as I already had pip installed from my [ProceduralCityGeneration Clone](https://github.com/pscheyer/ProceduralCityGeneration) project.

Had to modify directions- in the readme for the original it states

```bash
# Clone the repo
git clone https://github.com/dennybritz/rnn-tutorial-rnnlm
cd rnn-tutorial-rnnlm

# Create a new virtual environment (optional, but recommended)
virtualenv venv
source venv/bin/active

# Install requirements
pip install -r requirements.txt
# Start the notebook server
jupyter notebook
```

Incorrect instruction on line `source venv/bin/active`. Returns 
```bash
-bash: venv/bin/active: No such file or directory
```

Correct instruction is `source venv/bin/activate`, which creates a new virtual environment.

Also had to remove a space from my path to the file to get the command to run. I was getting the error 
```bash
(venv)Peters-MacBook-Pro:rnn-tutorial-rnnlm peterscheyer$ pip install -r requirements.txt
-bash: /Users/peterscheyer/Desktop/Python Projects/RecurrentNeuralNetworkTutorial/rnn-tutorial-rnnlm/venv/bin/pip: "/Users/peterscheyer/Desktop/Python: bad interpreter: No such file or directory
```
which is caused by the space in the folder name `Python Projects`. I replaced the space with an underscore and the requirements installation worked fine.

And the `jupyter notebook` command worked! For something. In my browser it opened a bunch of stuff… did I just start a server running? wtf is jupyter

20151001 1903CST

>The Jupyter Notebook is a web application that allows you to create and share documents that contain live code, equations, visualizations and explanatory text. Uses include: data cleaning and transformation, numerical simulation, statistical modeling, machine learning and much more

So there's that. I have one of those running now. 