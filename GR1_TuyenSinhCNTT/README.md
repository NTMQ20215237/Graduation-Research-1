#Here is my  RASA chatbot named "Tư vấn tuyển sinh Công nghệ thông tin".

To run this chatbot:

    - Requirement: 
    
        - Anaconda
        
        - Python=="version:3.8" or higher

    - First time running:
        - conda create -n NAME python==3.8 #Using anaconda to create a new virtual environment with python=="version:3.8"
                                               #Replace NAME to the name of the virtual environment
        - conda activate NAME                  #Activate the virtual environment

        - python -m pip uninstall pip
        - python -m ensurepip
        - python -m pip install -U pip         #Re-install pip 
        - pip install rasa                     #Install RASA using pip, here we must use RASA 3.0

        - rasa train                           #Train the chatbot  
        #You can also using "rasa --version" command to check if RASA is available or not.
        #Check if there is any issue with your RASA. The issue usually comes from your "SQLALchemy", your "Sanic" Framework.
        #Remember using these above commands in "Command Promt" Terminal which allows you to access to your virtual environment.

    - To run the chatbot: #Here you need to open at least 2 "Command Promt" Terminal which have access to the virtual environment.      
        - rasa run actions -v    #Run this command in the first terminal and keep this running
        Now comeback to the first terminal then running:
        - rasa shell            #Run the project. Now you can make question about IT
        
        

