# 🎮 Describe-and-Generate Game

This project implements a simple game where users can upload an image, which is then captioned by an AI model. The generated caption is then used to create a new image using another AI model.


## 🧩 Key Components

1. `app.py`: The main application file that sets up the Gradio interface and orchestrates the game flow.
2. `src/api/captioner.py`: Handles the image-to-text API calls and processing.
3. `src/api/generator.py`: Manages the text-to-image API calls and processing.
4. `src/utils/image_utils.py`: Contains utility functions for image processing.
5. `src/config.py`: Loads and manages environment variables and configuration settings.

## 🔄 Workflow

1. User uploads an image through the Gradio interface.
2. The `captioner` module processes the image and generates a descriptive caption.
3. The caption is displayed to the user and passed to the `generator` module.
4. The `generator` module creates a new image based on the caption.
5. The generated image is displayed to the user.

## 🚀 Setup

1. Clone the repository:
   ```
   git clone git clone https://github.com/Absorber97/AI-Image-Reimagine.git
   cd describe-and-generate
   ```

2. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

3. Create a `.env` file in the root directory with the following content:
   ```
   HF_API_KEY=your_huggingface_api_key
   HF_API_TTI_BASE=your_text_to_image_api_endpoint
   HF_API_ITT_BASE=your_image_to_text_api_endpoint
   ```

4. Run the application:
   ```
   python app.py
   ```

## 📖 Usage

1. Open the provided URL in your web browser.
2. Upload an image using the "Upload an image" button.
3. Click on "Caption and Generate" to get a caption for your image and generate a new image based on that caption.
4. Observe the AI-generated caption and the new image created from that caption.

## 🔑 API Configuration

This project uses Hugging Face's API for both image captioning and image generation. You need to set up an account on Hugging Face and obtain an API key. The specific endpoints for the Image-to-Text and Text-to-Image models should be configured in the `.env` file.

## 🐛 Error Handling and Logging

The application includes comprehensive error handling and logging to ensure smooth operation and easy debugging. Check the console output for detailed logs when running the application.

## 🤝 Contributing

We welcome contributions to the Describe-and-Generate Game! Here's how you can contribute:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

For major changes, please open an issue first to discuss what you would like to change.

## 🔮 Future Improvements

- Add support for multiple AI models for comparison
- Implement user accounts and history tracking
- Optimize image processing for faster performance
- Add more interactive elements to the game

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Hugging Face for providing powerful AI models and APIs
- Gradio team for the excellent web interface framework
- All contributors and supporters of the project
