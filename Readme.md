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