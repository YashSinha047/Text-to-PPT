# 🎯 Text-to-PPT – Auto-Generate PowerPoint Presentations from Text

**Transform Your Text into Professional Presentations – Instantly**

Text-to-PPT is a powerful web application that converts bulk text, markdown, or prose into fully formatted PowerPoint presentations while preserving your chosen template's visual style and layout. Simply paste your content, upload a template, and get a polished presentation ready for download.

<img width="1888" height="827" alt="image" src="https://github.com/user-attachments/assets/03e602e9-8f3b-4b06-a7d6-5c6379072ef5" />

---

## ✨ Features

* 📝 **Flexible Input**: Support for large text blocks, markdown, and long-form prose
* 🎯 **Smart Guidance**: Optional one-line instructions to control tone and structure (e.g., "create an investor pitch deck")
* 🔑 **Multi-LLM Support**: Compatible with OpenAI, Anthropic, Gemini, and other API providers (keys never stored)
* 🎨 **Template Preservation**: Upload `.pptx` or `.potx` files to maintain original colors, fonts, and layouts
* 🖼️ **Image Reuse**: Intelligently incorporates existing images from uploaded templates
* 📊 **Smart Content Mapping**: Automatically determines optimal slide count and content distribution
* 📥 **Instant Download**: Generate and download your presentation in seconds
* 🔒 **Privacy-First**: No storage or logging of user data, API keys, or uploaded files

---

## 🚀 Quick Start

### 1. Clone the Repository
```bash
git clone https://github.com/YashSinha047/Text-to-PPT.git
cd Text-to-PPT
```

### 2. Install Dependencies
```bash
# Install Python dependencies
pip install -r requirements.txt

# Frontend dependencies (if using Node.js build tools)
# npm install  # uncomment if applicable
```

### 3. Set Up Environment
```bash
# Copy environment template (if applicable)
cp .env.example .env

# Configure any necessary environment variables
```

### 4. Run the Application
```bash
# Start the development server
python app.py
# or
uvicorn main:app --reload
```

Visit: [http://localhost:8000](http://localhost:8000)

### 5. Deploy to Cloud
This application is deployment-ready for platforms like Railway, Render, Vercel, or Heroku. Simply connect your repository and deploy.

---

## 🖥️ How to Use

1. **Input Your Content**: Paste your text, markdown, or prose into the text area
2. **Add Guidance** (Optional): Provide a one-line instruction like *"make it a technical presentation"* or *"format as a sales pitch"*
3. **Enter API Key**: Paste your preferred LLM API key (OpenAI, Anthropic, Gemini, etc.)
4. **Upload Template**: Select your `.pptx` or `.potx` template file to define the visual style
5. **Generate**: Click the generate button and wait for processing
6. **Download**: Receive your styled PowerPoint presentation ready for use

---

## 🏗️ Technical Architecture

### Text Processing & Analysis
The application uses advanced LLM capabilities to:
- Parse and analyze input text structure and content themes
- Identify key sections, topics, and hierarchical information
- Determine optimal slide count based on content density and user guidance
- Extract and organize information into logical slide sequences

### Template Style Application
The system applies visual styling through:
- **Layout Mapping**: Analyzes template slide layouts and applies appropriate structures to new content
- **Style Inheritance**: Preserves fonts, colors, and formatting from uploaded templates
- **Image Integration**: Identifies and reuses existing images from templates where contextually appropriate
- **Asset Management**: Maintains template-specific design elements like backgrounds and themes

### Backend Architecture
* **Framework**: FastAPI for robust API handling and async processing
* **PowerPoint Generation**: `python-pptx` library for creating and manipulating presentation files
* **LLM Integration**: Flexible API client supporting multiple AI providers
* **File Processing**: Secure upload and processing of template files

### Frontend Features
* **Responsive Design**: Clean, modern interface built with Tailwind CSS
* **Real-time Feedback**: Progress indicators and status updates during processing
* **Error Handling**: Comprehensive error messages and validation
* **File Management**: Drag-and-drop upload with file type validation

---

## 🔧 Configuration

### Supported LLM Providers
- OpenAI GPT models
- Anthropic Claude
- Google Gemini
- Other OpenAI-compatible APIs

### File Specifications
- **Input Templates**: `.pptx`, `.potx` formats
- **Output**: Standard `.pptx` PowerPoint files
- **File Size Limits**: Configurable upload limits for optimal performance

---

## 🌟 Advanced Features

* **Speaker Notes Generation**: Automatically create presenter notes for each slide
* **Multiple Style Modes**: Support for different presentation types (professional, casual, technical)
* **Content Optimization**: Intelligent text summarization and bullet point extraction
* **Template Library**: Integration with common presentation templates
* **Batch Processing**: Handle multiple text inputs simultaneously
* **Export Options**: Multiple output formats and quality settings

---

## 🔒 Privacy & Security

- **Zero Data Retention**: No storage of user content, API keys, or uploaded files
- **Secure Processing**: All operations performed in memory with automatic cleanup
- **API Key Protection**: Keys used only for individual requests and never logged
- **HTTPS Enforcement**: Secure communication for all data transfers

---

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details on:
- Code style and standards
- Pull request process
- Issue reporting
- Feature requests

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🆘 Support

- **Issues**: Report bugs or request features via [GitHub Issues](https://github.com/YashSinha047/Text-to-PPT/issues)
- **Discussions**: Join community discussions in our [GitHub Discussions](https://github.com/YashSinha047/Text-to-PPT/discussions)

---

## 🙏 Acknowledgments

- Built with [python-pptx](https://python-pptx.readthedocs.io/) for PowerPoint generation
- Powered by state-of-the-art LLM APIs for intelligent content processing
- UI components styled with [Tailwind CSS](https://tailwindcss.com/)

---

**Ready to transform your text into professional presentations? Get started now!** 🚀
