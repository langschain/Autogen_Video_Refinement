# Autogen Video Refinement

The application is tailored to transform extended videos into succinct yet informative clips. It's a valuable tool for editors tasked with navigating through hours of footage, enabling them to streamline the process and craft engaging short films or highlight reels more efficiently.
## Features


1. **📥 Download Video:** Downloads a video file from a provided link.
2. **🗣️ Speech Recognition:** Utilizes the whisper model to extract utterances from the video and converts them to text, saving the transcription as a script file.
3. **⏱️ Video Duration:** Determines the duration of the video.
4. **📝 Short Transcription:** Creates a short transcription from the full transcription that highlights the best parts of the video.
5. **🎥 Short Video** Creation: Creates a short video by joining segments from the original video based on the short transcription.

## Tecnologies Used:

1. [**MoviePy**](https://pypi.org/project/moviepy/) - Video editing library
2. [**PyAutoGen**](https://microsoft.github.io/autogen/) - Library for automating software tasks. (Microsoft Autogen)
3. [**Whisper**](https://github.com/openai/whisper) - Automatic speech recognition model
4. [**OpenAI**](https://openai.com/) - API for interacting with OpenAI services.

## Installation
**Prerequisites:**

*   **Python (3.7 or later):** Download and install Python from [https://www.python.org/downloads/](https://www.python.org/downloads/) if you haven't already.
    
*   **Virtual Environment (Recommended):** It's highly recommended to create a virtual environment to isolate project dependencies. Here's how to create one using `venv`:
    
    Bash
    
        python -m venv venv
        source venv/bin/activate  # macOS/Linux
        venv\Scripts\activate.bat  # Windows

**Installation:**

1.  **Clone the Repository:** Use `git` to clone the project from GitHub:
    
    Bash
    
        git clone https://github.com/langschain/Autogen_Video_Refinement.git
        cd Autogen_Video_Refinement
    
2.  **Install Dependencies:** Navigate to the project directory and install required packages using `pip`:
    
    Bash
    
        pip install -r requirements.txt
    
    This will install `autogen`, `whisper`, `moviepy`, `requests`, `openai`, `pydantic`, and `dotenv`.
    

**Optional: API Keys**

*   **OpenAI API Key:** If you plan to use OpenAI's GPT-3 functionality, obtain an API key from [https://beta.openai.com/account/api-keys](https://beta.openai.com/account/api-keys) and set the `OPENAI_API_KEY` environment variable in your `.env` file (create one if it doesn't exist).

**Running the Application:**

1.  **Create a `.env` File (Optional):**
    
    *   Create a file named `.env` in the project's root directory.
        
    *   Add any environment variables required by the project, such as `OPENAI_API_KEY`. For example:
        
        OPENAI_API_KEY=your_openai_api_key
        
2.  **Load Environment Variables:**
    
    *   Uncomment the `load_dotenv()` line at the beginning of the `main.py` script to load variables from the `.env` file.
3.  **Execute the Script:**
    
    *   Run the `main.py` script using Python:
        
        Bash
        
            python main.py
    ![image](https://github.com/langschain/Autogen_Video_Refinement/assets/100914015/51221352-d6aa-4b76-8e58-e97001d955e8)

**Additional Notes:**

*   The code includes comments and docstrings to enhance readability.
*   Consider using a linter or code formatter to maintain consistent style.

## Usage

Add a video url in the autogen's final prompt.
Sample Video Link
```
https://github.com/langschain/Autogen_Video_Refinement/raw/master/sample_video.mp4
```


## License

[MIT License](https://opensource.org/license/mit)

Copyright (c) [2024] [Langschain / Autogen Video Refinement]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

