# Cable Sag Prediction using AI in Grasshopper

In this project, I built a simple model to predict **cable sag**. 💡

![Grasshopper Script](IMG_0691.jpeg)

### The workflow was pretty straightforward:
First, I generated about 25 training samples using the **Kangaroo** plugin.

Here are the variables:
🔸 **Inputs:** Span, Cable Length, and Gravity (Load)  
🔹 **Output:** Cable Sag  

Then, I used the **Galapagos** evolutionary algorithm to train the model and minimize the prediction error. 🎯 

Finally, I tested it with entirely new data. Even with just 25 training samples, the results for this simple model were surprisingly accurate and impressive!

---

### 🛠️ Tools Used:
* **Rhinoceros 3D / Grasshopper**
* **Kangaroo Physics** (for data generation)
* **Galapagos** (for model optimization)
