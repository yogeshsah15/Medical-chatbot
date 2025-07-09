# End-to-End Medical Chatbot with Generative AI

This project implements an end-to-end medical chatbot powered by Generative AI. The chatbot assists users with medical inquiries by providing accurate and context-aware responses. It leverages state-of-the-art AI models and integrates seamlessly with a backend API for enhanced functionality.

---

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Project Structure](#project-structure)
- [Setup and Installation](#setup-and-installation)
- [Usage](#usage)
- [Dependencies](#dependencies)
- [Contributing](#contributing)
- [License](#license)

---

## Project Overview

The medical chatbot is built using modern AI technologies, including natural language processing (NLP) and generative AI models. It is designed to:
- Understand user queries in natural language.
- Provide accurate and contextually relevant medical information.
- Offer a user-friendly interface for interaction.

---

## Features

- **Generative AI Integration**: Utilizes advanced AI models for generating responses.
- **Medical Knowledge Base**: Trained on a dataset of medical information.
- **Interactive Chat Interface**: User-friendly interface for seamless interaction.
- **Scalable Backend**: API-driven architecture for scalability.
- **Customizable**: Easily extendable to include additional features or integrate with external systems.

---

## Project Structure

```
End-to-End-Medical-Chatbot-Generative-AI/
├── src/
│   ├── models/          # AI models and training scripts
│   ├── api/             # Backend API implementation
│   ├── utils/           # Utility functions and helpers
│   ├── config/          # Configuration files
│   └── app.py           # Main application entry point
├── data/
│   ├── training_data/   # Dataset for training the AI model
│   └── processed_data/  # Preprocessed data
├── tests/               # Unit and integration tests
├── docs/                # Documentation and resources
├── requirements.txt     # Python dependencies
├── README.md            # Project documentation
└── LICENSE              # License information
```

---

## Setup and Installation

### Steps:

1. **Clone the repository**  
	```bash
	git clone https://github.com/your-repo-url.git
	cd End-to-End-Medical-Chatbot-Generative-AI
	```

2. **Prepare the dataset**  
	Place your dataset in the `data/training_data/` directory.

3. **Create a conda environment**  
	```bash
	conda create -n myenv python=3.10 -y
	conda activate myenv
	```

4. **Install the requirements**  
	```bash
	pip install -r requirements.txt
	```

5. **Set up environment variables**  
	Create a `.env` file in the root directory and add your Pinecone & OpenAI credentials:
	```env
	PINECONE_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
	OPENAI_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
	```

6. **Store embeddings to Pinecone**  
	```bash
	python store_index.py
	```

7. **Run the application**  
	```bash
	python app.py
	```

8. **Access the application**  
	Open your browser and navigate to `http://localhost:`.

---

## Usage

1. Start the application using the command above.
2. Access the chatbot interface via the provided URL (e.g., `http://localhost:2000`).
3. Interact with the chatbot by typing your medical queries.

---

## Dependencies

The project uses the following key dependencies:
- **Flask**: For building the backend API.
- **Transformers**: For leveraging pre-trained generative AI models.
- **Pandas**: For data manipulation and preprocessing.
- **Scikit-learn**: For additional machine learning utilities.

Refer to `requirements.txt` for the complete list of dependencies.

---

## Contributing

Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Submit a pull request with a detailed description of your changes.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

Feel free to reach out with any questions or suggestions!  
