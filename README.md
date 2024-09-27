# WhatsApp Chat Analyzer

A Streamlit-based web application for analyzing WhatsApp chat data. This tool allows users to upload their WhatsApp chat history and visualize key statistics, timelines, activity maps, most common words, and emoji usage. It is designed to offer insights into both individual and group chats, making the analysis of conversations interactive and insightful.

## Features

- **Upload WhatsApp Chat File**: Easily upload the exported `.txt` file of your WhatsApp conversation.
- **User-specific or Overall Analysis**: Choose to analyze data for a specific user or the entire chat.
- **Top Statistics**:
  - Total Messages
  - Total Words
  - Media Shared
  - Links Shared
- **Message Timelines**:
  - Monthly and daily message frequency visualized through line charts.
- **Activity Maps**:
  - See which days of the week and which months were the most active using bar charts and heatmaps.
- **Busiest Users**: Identify the most active participants in a group chat.
- **Word Cloud**: Visualize the most common words in the conversation.
- **Most Common Words**: Display the most frequently used words with bar charts.
- **Emoji Analysis**: Explore the emojis used, with a pie chart showing their distribution.

## Code Structure

The project contains three main files:

1. **`app.py`**:
   - The main Streamlit application that handles user interaction and visualization of the chat data.
   
2. **`helper.py`**:
   - Contains helper functions for data processing and visualization such as:
     - Fetching statistics for messages, words, media, and links.
     - Generating word clouds and identifying the most common words.
     - Analyzing emoji usage and creating activity maps and timelines.
   - Example functions:  `fetch_stats()`, `most_busy_users()`, `create_wordcloud()`, `emoji_helper()`, and more&#8203;:contentReference[oaicite:0]{index=0}.
   
3. **`preprocessor.py`**:
   - Handles the preprocessing of the uploaded chat data:
     - Cleans and structures raw text data into a DataFrame.
     - Extracts user names, message content, dates, and other relevant information.
     - Example function: `preprocess()`&#8203;:contentReference[oaicite:1]{index=1}.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-repo/whatsapp-chat-analyzer.git
   cd whatsapp-chat-analyzer
2. Install the required dependencies
3. Run the Streamlit app:
   ```bash
   streamlit run app.py

## How to Use
1. Export your WhatsApp chat in .txt format.
2. Upload the file using the sidebar in the app.
3. Select a specific user or "Overall" for group analysis.
4. Click on "Show Analysis" to view various statistics and visualizations.

## Dependencies
- Streamlit: For building the web interface.
- Matplotlib: For generating plots and visualizations.
- Seaborn: For creating heatmaps.
- Pandas: For data manipulation and preprocessing.
- WordCloud: For generating word clouds.
- URLEXtract: For extracting URLs from messages.
- Emoji: For emoji analysis.

## Screenshots
![benchmark](https://github.com/MorshedulHoque/WhatsApp-Data-Analyzer/blob/main/Dashboard/Screenshot_1.png)
![benchmark](https://github.com/MorshedulHoque/WhatsApp-Data-Analyzer/blob/main/Dashboard/Screenshot_2.png)
![benchmark](https://github.com/MorshedulHoque/WhatsApp-Data-Analyzer/blob/main/Dashboard/Screenshot_3.png)
![benchmark](https://github.com/MorshedulHoque/WhatsApp-Data-Analyzer/blob/main/Dashboard/Screenshot_4.png)

