# Speech-to-Text Converter 🎤📝

A Python-based audio transcription tool that converts speech from various audio formats to text using Google's Speech Recognition API.

## ✨ Features

- **Multi-format Support**: Handles WAV, MP3, M4A, OGG, and FLAC audio files
- **Automatic Format Conversion**: Seamlessly converts unsupported formats to WAV for processing
- **Language Flexibility**: Supports multiple languages through language code specification
- **File Output**: Saves transcriptions directly to text files
- **Clean Architecture**: Modular design with separate functions for each core operation

## 🚀 Quick Start

### Prerequisites

Install the required Python packages:
- speechrecognition
- pydub

**Note**: For MP3 support, you may need ffmpeg installed on your system.

### Usage

1. **Run the script**
2. **Follow the interactive prompts**:
   - Enter the path to your audio file
   - Specify the output text file path
   - Provide language code (e.g., en-US, es-ES, fr-FR)

The application will process your audio file and display the transcribed text while also saving it to your specified output file.

## 🏗️ How It Works

The application follows a streamlined workflow:

### Core Components

The project is built around four main functions that handle different aspects of the transcription process:

- **Audio Preparation**: Validates and converts audio files to the required WAV format when needed
- **Speech Recognition**: Utilizes Google's API to convert audio data into text
- **File Management**: Handles reading audio files and writing transcription results
- **Process Orchestration**: Coordinates the entire workflow from input to output

### Unique Implementation Details

- **Smart Format Detection**: Automatically identifies audio file formats and only converts when necessary
- **Conditional Processing**: Skips conversion for files already in WAV format to save processing time
- **Interactive Interface**: User-friendly command-line prompts guide users through the process
- **Robust Error Handling**: Comprehensive validation and error management for various failure scenarios

## 📋 Supported Languages

The application supports multiple languages for transcription. Use the appropriate language codes when prompted:

- English (US, UK)
- Spanish (Spain)
- French (France)
- German (Germany)
- Italian (Italy)
- Portuguese (Brazil)
- Japanese
- Korean
- Chinese (Simplified)
- And many more supported by Google's Speech Recognition API

## 🛠️ Technical Requirements

- **Python 3.6+**
- **Internet Connection**: Required for Google Speech Recognition API
- **Audio File Formats**: WAV, MP3, M4A, OGG, FLAC


## 🔧 Error Handling

The application handles several error scenarios:

- **File Not Found**: Validates input file existence
- **Unsupported Format**: Raises clear error for invalid audio formats
- **API Errors**: Catches and reports speech recognition failures
- **Permission Issues**: Handles file read/write permission problems

## 🙏 Acknowledgments

- Google Speech Recognition API for speech-to-text capabilities
- PyDub library for audio format conversion
- SpeechRecognition library for Python integration

