# AgenticAI_VideoSummarizer
# Phidata Video AI Summarizer Agent 🎥🎤🖬

This Streamlit application uses the Phidata Agent framework, powered by Google's Gemini 2.0 Flash Exp model, to analyze and summarize video content. It allows users to upload video files and ask questions about the video, leveraging both the video content and supplementary web research through DuckDuckGo.

## Features

-   **Video Upload:** Users can upload video files (MP4, MOV, AVI).
-   **AI-Powered Analysis:** The application uses the Gemini 2.0 Flash Exp model to analyze the video content.
-   **Contextual Question Answering:** Users can ask questions about the video, and the AI agent will provide detailed, user-friendly, and actionable responses.
-   **Web Research:** The agent uses DuckDuckGo for supplementary web research to enhance the analysis.
-   **Streamlit Interface:** A user-friendly web interface built with Streamlit.
-   **Temporary File Handling:** Uses tempfiles to process uploaded videos, and cleans up the files after processing.
-   **Environment Variable API Key:** Uses .env files to store API keys.

## Prerequisites

-   Python 3.x
-   Google Cloud Platform (GCP) account with the Generative Language API enabled.
-   A valid Google API key.
-   `pip` package manager.

## Installation

1.  **Clone the repository:**

    ```bash
    git clone <repository_url>
    cd <repository_directory>
    ```

2.  **Create a virtual environment (recommended):**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On macOS/Linux
    venv\Scripts\activate  # On Windows
    ```

3.  **Install dependencies:**

    ```bash
    pip install streamlit phi google-generativeai python-dotenv
    ```

4.  **Set up your API key:**

    -   Create a `.env` file in the same directory as your Python script.
    -   Add your Google API key to the `.env` file:

        ```
        GOOGLE_API_KEY=YOUR_ACTUAL_API_KEY
        ```

    -   Replace `YOUR_ACTUAL_API_KEY` with your actual API key.

5.  **Run the Streamlit application:**

    ```bash
    streamlit run app.py
    ```

    (Replace `app.py` with the name of your python file.)

## Usage

1.  Open the Streamlit application in your web browser.
2.  Upload a video file using the file uploader.
3.  Enter your question or desired insights in the text area.
4.  Click the "🔍 Analyze Video" button.
5.  The AI agent will process the video and display the analysis result.

## Example

-   Upload a video of a presentation.
-   Ask: "What were the main points of the presentation?"
-   The agent will summarize the key takeaways from the video.

## Dependencies

-   Streamlit
-   Phidata Agent
-   Google Generative AI
-   python-dotenv

## Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues.

## License

[Your License (e.g., MIT)](LICENSE)