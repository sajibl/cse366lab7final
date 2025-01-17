# Caltech-101 Classification Model

Training completed with:
- Number of classes: 102
- Final training accuracy: 71.55%
- Final validation accuracy: 64.00%

Files included:
- final_model.pth: Trained PyTorch model
- training_history.json: Training metrics history
- training_curves.png: Visualization of training progress
- gradcam_visualizations.png: Grad-CAM visualizations

To load the model:
```python
import torch
checkpoint = torch.load('final_model.pth')
model.load_state_dict(checkpoint['model_state_dict'])
class_names = checkpoint['class_names']
```
