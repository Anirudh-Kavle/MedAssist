# MedAssist

## Project Description

The SRM Global Hospital Medical Bot is an application developed to assist healthcare professionals at SRM Global Hospital. This bot utilizes Llama3 and machine learning techniques to provide accurate and timely responses to medical queries based on the hospital's specific health guidelines. The project was initiated when doctors from SRM Global Hospital approached the engineering department with the idea of developing a medical bot that could answer questions using the hospital's unique health guidelines. This solution addresses the challenges of potential oversight, contradictory suggestions, and the need for quick access to standardized information.

## Key Features

- **Document Embedding**: Utilizes OpenAI embeddings to create a searchable vector database of the hospital's health guidelines.
- **Natural Language Query Processing**: Powered by the Llama3-8b-8192 model through the Groq API for advanced language understanding and generation.
- **Context-Aware Responses**: Provide answers based on the most relevant sections of the health guidelines.
- **User-Friendly Interface**: Built with Streamlit for an intuitive and easy-to-use experience.
- **Real-time Information Retrieval**: Quickly retrieves and presents relevant information from the embedded documents.
- **Expandable Knowledge Base**: Easily update the system with new guidelines by adding PDFs to the data directory.

## Dependencies

To run this project, you'll need the following API keys:

- Groq API Key
- OpenAI API Key

Ensure these are set in your `.env` file.

## Setup

1. Clone the repository:
   ```
   git clone https://github.com/Anirudh-Kavle/MedAssist.git
   cd MedAssist
   ```

2. Install the required packages:
   ```
   pip install -r req.txt
   ```

3. Create a `.env` file in the project root and add your API keys:
   ```
   GROQ_API_KEY=your_groq_api_key_here
   OPENAI_API_KEY=your_openai_api_key_here
   ```

4. Place your PDF documents containing the health guidelines in the `./data` directory.

5. Run the Streamlit app:
   ```
   streamlit run app.py
   ```
