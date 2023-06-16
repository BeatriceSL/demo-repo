**Promethean Fire AI**: Revolutionizing physician documentation

Promethean Fire AI is an advanced tool that enables you to effectively monitor physician sessions, whether they are conducted virtually or in-person. Our state-of-the-art AI system listens to the sessions in real-time, transcribes the conversations, and captures comprehensive notes. Through a real-time dashboard, you'll gain valuable insights into the important topics and entities discussed during the session, allowing you to prioritize the well-being of your patients.
As the conversations progress and topics shift, Promethean Fire AI dynamically highlights key subjects and entities, ensuring that you never overlook critical information. After the session, you can easily download a customized summary of the session notes and the complete transcript, simplifying your documentation process and enabling you to provide tailored support for your clients.
Under the hood, Promethean Fire AI relies on a Python backend and a sleek HTML/JavaScript frontend. The robust Python backend is built using the FastAPI framework and integrates various AI models, including:

Deepgram: for real-time audio transcription and speaker identification
OpenAI’s GPT-3.5-turbo: for entity and topic modeling, summarization, and extraction
Deepgram streams audio transcriptions in manageable chunks, while the backend accumulates and sends them to GPT-3.5-turbo in batches. The backend then seamlessly streams the results from both the transcription and language model back to the client using an event-stream, effortlessly displaying the outcomes in the user interface.
Embrace the transformative potential of Prometheus Fire AI and join the revolution and enhance your sessions today. To run this project, create a virtual environment by executing the provided commands. You can find further information on setting up a virtual environment in the documentation.

[article](https://developers.deepgram.com/blog/2022/02/python-virtual-environments/).

```
mkdir [% NAME_OF_YOUR_DIRECTORY %]
cd [% NAME_OF_YOUR_DIRECTORY %]
python3 -m venv venv
source venv/bin/activate
```

Make sure your virtual environment is activated and install the dependencies in the requirements.txt file inside.

```
pip install -r requirements.txt
```

Add API key :
`export DEEPGRAM_API_KEY=968957b825a693b5c0e7cbd2e9282e01d0120592`

Make sure you're in the project root directory and run the project in the development server.

```
uvicorn src.main:app --reload
```

Pull up a browser and go to your localhost, http://127.0.0.1:8000/.

Allow access to your microphone and start speaking. A transcript of your audio will appear in the browser.

License

When you are using Typescript ? Make sure it makes you faster. 

Step 1. Start with Demo video people can see
Step 2. Pitch Deck with Background

We could use a way to use Open Source models without exposing our in-house data.
