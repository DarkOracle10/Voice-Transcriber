# Changelog - Persian Audio Transcriber

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2025-12-13

### Added
- Persian/Farsi language support with Hazm text normalization
- GPU acceleration support (CUDA/FP16) for NVIDIA RTX GPUs
- Multiple transcription engines:
  - OpenAI Whisper
  - Faster-Whisper (optimized)
  - OpenAI API
  - Google Speech Recognition
- Batch folder processing capability
- Multiple output formats:
  - Plain text (TXT)
  - JSON with detailed metadata
  - SRT subtitle files
- Support for multiple audio/video formats:
  - MP3, MP4, WAV, M4A, FLAC, OGG, AAC, WMA
- Automatic audio extraction from MP4 video files
- Persian text normalization:
  - Arabic to Persian character conversion
  - Whitespace normalization
  - Text cleanup
- Automatic CUDA DLL path detection (Windows)
- CPU fallback when GPU unavailable
- Command-line interface with comprehensive options
- Python API for programmatic use
- Progress tracking for batch processing
- Error handling with automatic fallback
- Comprehensive documentation

### Performance
- GPU acceleration provides 5-10x speedup on RTX GPUs
- FP16 precision for faster inference with minimal accuracy loss
- Optimized Faster-Whisper engine for best performance

### Technical
- Automatic PATH management for CUDA DLLs
- Cross-platform compatibility (Windows, Linux, macOS)
- Virtual environment support
- Requirements file for easy dependency management
- Setup.py for pip installation

### Documentation
- Comprehensive README.md
- User guides
- API documentation
- Troubleshooting guide
- Usage examples

## [1.0.1] - 2025-12-15

### Changed
- **Project renamed** to `persian-audio-transcriber` for better clarity
- **CLI command** renamed from `voice-transcriber` to `persian-transcriber`
- Updated all documentation to reflect new project name
- Updated repository URLs to `https://github.com/DarkOracle10/persian-audio-transcriber`
- Updated package names in setup.py and pyproject.toml

### Improved
- Enhanced .gitignore to properly exclude only generated files
- Added comprehensive project structure documentation
- Updated all API documentation references
- Improved ARCHITECTURE.md with project name
- Enhanced PROJECT_SUMMARY.md with complete project details

### Fixed
- Corrected all repository URLs across documentation
- Fixed console script names in packaging files
- Updated config.yaml with correct project name

## [Unreleased]

### Planned
- Web interface (Flask/FastAPI)
- Real-time transcription
- Multi-language support (beyond Persian)
- Docker containerization
- REST API endpoints
- Database integration for transcription storage
- Frontend dashboard for transcription management

