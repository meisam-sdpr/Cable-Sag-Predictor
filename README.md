# Cable Sag Predictor

In this project, I built a simple data-driven model that predicts **cable sag**
from a few design parameters. In effect, it's a lightweight **surrogate model**
that approximates the Kangaroo physics simulation — once fitted, it estimates
sag instantly, without re-running the simulation. 💡

![Grasshopper Script](IMG_0691.jpeg)

### The workflow was pretty straightforward:
First, I generated about 25 training samples using the **Kangaroo** plugin.

Here are the variables:
🔸 **Inputs:** Span, Cable Length, and Gravity (Load)  
🔹 **Output:** Cable Sag  

Then, I used the **Galapagos** evolutionary algorithm to **fit the model** and
minimize the prediction error against the dataset.🎯 

Finally, I tested it with entirely new data. Even with just 25 training samples, the results for this simple model were surprisingly accurate and impressive!

---

### 🛠️ Tools Used:
* **Rhinoceros 3D / Grasshopper**
* **Kangaroo Physics** (for data generation)
* **Galapagos** (for model optimization)
