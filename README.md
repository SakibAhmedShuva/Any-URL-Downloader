# Any-URL-Downloader

A robust Python utility for extracting and downloading files from URLs found in various text-based documents.

## Features

- 📝 Supports multiple file formats (JSON, TXT, MD, CSV)
- 🔍 Smart URL detection and extraction
- 📊 Concurrent downloads using thread pooling
- 🎯 Automatic file type detection and extension assignment
- 💪 Robust error handling and progress tracking
- 🚀 Support for both single files and directories

## Installation

1. Clone the repository:
```bash
git clone https://github.com/SakibAhmedShuva/Any-URL-Downloader
cd url-downloader
```

2. Install required dependencies:
```bash
pip install -r requirements.txt
```

## Usage

### As a Python Script

```python
from url_downloader import process_files

# Process a single file
process_files("path/to/your/file.json", "output_directory")

# Process an entire directory
process_files("path/to/directory", "output_directory")
```

### Command Line Usage

```bash
python url_downloader.py
```

## Configuration

The script includes several configurable parameters:

- `max_workers`: Number of concurrent download threads (default: 5)
- `supported_extensions`: File types that can be processed (.json, .txt, .md, .csv)
- `timeout`: Download timeout in seconds (default: 30)

## Features in Detail

### URL Extraction
- Supports complex URL patterns
- Validates URLs before processing
- Handles URL-encoded characters

### File Download
- Automatic content-type detection
- Progress tracking
- Robust error handling
- Sanitized filename generation

### Concurrent Processing
- Thread pool implementation
- Configurable worker count
- Download status tracking

## Requirements

- Python 3.6+
- requests
- urllib3

## Project Structure

```
url_downloader/
│
├── url_downloader.ipynb      # Main implementation
├── requirements.txt          # Project dependencies
└── README.md                # Documentation
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Thanks to all contributors
- Inspired by the need for efficient URL extraction and download management

## Author

Your Name - [@yourgithub](https://github.com/yourusername)

## Support

If you encounter any issues or have questions, please file an issue on the GitHub repository.
