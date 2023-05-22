# LooresGptChatBotTest
deployment of an gpt chat in linux 



1.- In order to deploy this GPT chat robot, the following preconditions must be fulfilled 

//==Install Python==//

sudo apt install python3
sudo apt install python3-pip
sudo apt install python3-venv

//==verification==//

python3 --version
pip3 --version


Now that you have the dependencies covered, let’s create the environment to access ChatGPT

mkdir LoorsGptChat
cd    LoorsGptChat

Now, use the command below to create a virtual environment with the venv module. We have used the “chatloorsgpt_cli” name for our virtual environment.

python3 -m venv chatloorsgpt_cli
source chatloorsgpt_cli/bin/activate

If Linux shell prompt changed to (chatloorsgpt_cli), the virtual enviroment was created correctly.

2.- The Gpts deployment needs an api to communicate and proccess the information, so one apy key is needed

//==url to get the api==//
https://openai.com/

-create an account
-now click your profile pic and look for the 'view api keys'  title , then click it.
-you will get a sk-************** secret key, that we are going to replace in the source code named or by setting it as a enviroment variable we can call it, in an easier way

//==setting enviroment variable==//

export OPENAI_API_KEY=sk***************

if wanted this envioment variable can be stored as a regular one as the followin way

export OPENAI_API_KEY=<your_OpenAI_API_key_here> // under the .bash so if needed type the followin command

//==setting as a permanent enviroment variable (if needed)==//

sudo nano /home/'your username'/.bashrc
export OPENAI_API_KEY=sk*********

we can check that everything go thrue as follow

//==verify==//
env

to complete the preconditions is necesary to install the 'shell-gpt' pkg as follow

pip3 install shell-gpt --user

now we need to connect our char gpt to the whatsapp or telegram 

//==url to connect the telegrar or whatsapp chat manager==//
https://buddygpt.ai/ref/davinder


the tap in the button "get for whatsapp" or "get for telegram"


