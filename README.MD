## AI Email Generator

<p align = "center"><img src = "./assets/email_writer.gif" height = 300 alt = "Wallet Icon"></p>

A minimalistic application to generate custom email templates built using Python and GPT-3



## Set-Up ⚒️

<p align = "center"><img src = "./assets/setup.gif" height = 300 alt = "SetUp Icon"></p>

- Ensure you have the latest stable version of [Python](https://www.python.org/downloads/) in your system

- Open your terminal / command prompt. 

- Clone the repository 
    ```
    git clone https://github.com/smaranjitghose/AIEmailGenerator.git
    ```
- Change the directory to the cloned project
    
    ```
    cd AIEmailGenerator
    ```

- Create a virtual environment

    ```
    python -m venv env
    ```

- Activate the virtual environment

    - Windows
        ```
         env/Scripts/Activate.ps1
        ```
    
    - Linux/Mac
        ```
        source env/bin/activate
        ```

- Check if the virtual environment in the concerned repository is used for python shell

    ```
    which python
    ```

- Upgrage Pip Installer

    ```
    python -m pip install --upgrade pip
    ```

- Install the dependencies

    ```
    pip install -r requirements.txt
    ```

- Load the application

    ```
    streamlit run .\Home.py
    ```

- If the app does not load by itself in your default browser, open a browser of your choice and navigate to  `http://localhost:8501`

- To stop the application, press `CTRL + C` in your terminal

- To deactive the python environment, type in your terminal

    ```
    deactivate
    ```

## Demo 👇

**v.0.0.1**


<p align = "center"><img src = "./assets/demo_snapshot_v1_1.png" height = 300 width = 450 alt = "AITranscriber Snapshot v1"></p>

**v.0.0.1** (Sample Email)
<p align = "center"><img src = "./assets/demo_snapshot_v1_2.png" height = 300 width = 450 alt = "AITranscriber Snapshot v1"></p>


## Note ✏️

<p align = "center"><img src = "./assets/notes.gif" height = 300 alt = "Note Icon"></p>


- For Streamlit Sharing, mentioning versions of the modules in requirements throws error at times


## Future Work 🏗️

- [ ] Chrome Plugin
- [ ] Better Prompting
- [ ] Editable
- [ ] Sample Templats: 10
- [ ] Add to Email



## Deployment Options 🥊

<p align = "center"><img src = "./assets/hosting.gif" height = 300 alt = "Hosting Icon"></p>

- [Streamlit Cloud](https://streamlit.io/cloud)
- [HuggingFace Spaces](https://huggingface.co/docs/hub/spaces)

- [Fly](https://fly.io/)
- [Railway](https://railway.app/)
- [Render](https://render.com/)
- [Cyclic](https://app.cyclic.sh/#/)

- [Heroku](https://www.heroku.com/)
- [Digital Ocean](https://www.digitalocean.com/)

- Google App Engine
- Amazon EC2 Instance
- Azure App

(**Using Google Colab/Kaggle as temporary MVP server**)

- [pyngrok](https://pyngrok.readthedocs.io/en/latest/index.html)
    - Step 1: Install pyngrok in Google Colab

        ```
        ! pip install pyngrok
        ```
    
    - Step 2: Sign-up in [ngrok](https://ngrok.com/) and get Authentication Token

    - Step 3: Authenticate
        
        ```python
           from pyngrok import ngrok
           ngrok.set_auth_token("xxx")
        ```
    - Step 4: Load the Streamlit App at port 8051, create a tunnel for it and reveal the public URL for the tunnel

        ```python
           !nohup streamlit run app.py --server.port 8051 &
           url = ngrok.connect(8051).public_url
           print(url)
        ```
    
    - Step 5: Share URL with client
     


- [localtunnel](https://github.com/localtunnel/localtunnel)
    - Step 1: Install localtunnel

        ```
        npm install -g localtunnel
        ```
    - Step 2

        ```
        streamlit run Home.py & npx localtunnel --port 8501
        ```
    
    - Step 3: Share URL with client

## Acknowledgements 🙏

<p align = "center"><img src = "https://media.giphy.com/media/1gQ6f5kJdBtGPSmdgS/giphy.gif" height = 300 alt = "Acknowledgment Icon"></p>


- **Text to Text Generator Model**: [OpenAI GPT3](https://openai.com/blog/gpt-3-apps/) 
    - [Documentation](https://beta.openai.com/docs/)
    - [Playground](https://beta.openai.com/playground)
- **Animations**: [LottieFiles](https://lottiefiles.com)
