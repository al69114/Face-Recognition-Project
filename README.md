YouTubeFaceFinder

- YouTubeFaceFinder is a Python tool that automatically detects and extracts unique faces from YouTube videos—including Shorts, static comparison videos, and dynamic content. It intelligently distinguishes between static, dynamic, and mixed videos, applying optimized face detection and recognition strategies for each case.


Features

Robust Face Detection:
Utilizes MTCNN for multi-scale, multi-preprocessing face detection—even on small faces in YouTube Shorts.

Deep Face Recognition:
Uses FaceNet (InceptionResnetV1) for embedding-based face recognition and deduplication.

Unique Face Extraction:
Only saves unique faces using cosine similarity between embeddings, preventing duplicates across frames and segments.

Preprocessing for Challenging Content:
Handles low-light, blurry, or small faces with upscaling, contrast enhancement, histogram equalization, and sharpening.

Batch Processing & Progress Bars:
Efficiently processes long videos with progress feedback.

Output Organization:
Saves frames, all detected faces, and unique faces in structured folders for easy review.

Install dependencies:

pip install facenet-pytorch opencv-python numpy scipy matplotlib tqdm scikit-learn
pip install yt-dlp
