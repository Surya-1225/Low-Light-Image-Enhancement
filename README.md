Real-Time Image Enhancement using CLAHE and Gamma Correction
📌 Overview

This project implements a real-time image enhancement system using classical image processing techniques.
It captures live video from a webcam, enhances each frame using contrast and brightness adjustments, and evaluates the enhancement quality using PSNR and SSIM metrics.
The system displays the original and enhanced frames side-by-side along with real-time quality measurements.

==================================================================================

🚀 Features

📷 Real-time webcam video capture

🌗 Contrast enhancement using CLAHE

☀️ Brightness adjustment using Gamma Correction

📊 Quality evaluation using:
    PSNR (Peak Signal-to-Noise Ratio)
    SSIM (Structural Similarity Index)
    
🖥️ Side-by-side comparison display

==================================================================================

🧠 Working Principle:
1️⃣ Contrast Enhancement (CLAHE)
        Converts image from BGR to YUV color space
        Applies CLAHE (Contrast Limited Adaptive Histogram Equalization) on the luminance (Y) channel
        Improves local contrast while preventing over-amplification of noise

2️⃣ Gamma Correction:
        Applies nonlinear brightness transformation
        Uses a lookup table for fast pixel intensity adjustment
        Enhances visibility in darker regions

3️⃣ Quality Metrics:
        PSNR measures pixel-level difference between original and enhanced images
        SSIM evaluates structural similarity
        
==================================================================================

🛠️ Technologies Used
      Python
      OpenCV
      NumPy
      scikit-image
      Math library
      
==================================================================================

📈 Output
      Left side → Original Frame
      Right side → Enhanced Frame
      Top overlay → PSNR and SSIM values
      
==================================================================================

📊 Sample Enhancement Pipeline:


                                      Webcam Input
                                           ↓
                                      Resize Frame
                                           ↓
                                      CLAHE (Y Channel)
                                           ↓
                                      Gamma Correction
                                           ↓
                                      Compute PSNR & SSIM
                                           ↓
                                      Display Comparison


==================================================================================

🎯 Applications:
      Low-light video enhancement
      Surveillance preprocessing
      Computer vision preprocessing pipeline
      Academic demonstration of classical image enhancement techniques
      
==================================================================================

⚠️ Note

Since the goal is enhancement (not reconstruction), PSNR and SSIM values may decrease even if visual quality improves. These metrics should be interpreted carefully.




      
