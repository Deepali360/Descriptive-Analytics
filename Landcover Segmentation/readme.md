### **Overview**  
This project explores image segmentation for large satellite images with class imbalance using **UNet++** and **DeepLabV3+** architectures. Both models were trained on Poland’s satellite RGB images with five classes, using **ResNet15** as the backbone and **ImageNet weights**.  

### **Key Findings**  
- **UNet++** achieved better segmentation accuracy (higher Dice score).  
- **DeepLabV3+** demonstrated better computational efficiency.  
- **Best segmentation** results were for **woodlands** and **water**, but **narrow structures** like roads and buildings remained challenging.  
- Our model outperformed benchmarks, achieving **84-85% mean IoU** on a relatively small dataset.  

🚀 **Future Work:** Further fine-tuning and additional data augmentation to improve segmentation of narrow regions.
