# Logistic-Regression-ML-Algorithm

### 🤖 What Is Logistic Regression?

**Logistic Regression** is a statistical and machine learning algorithm used for binary classification problems — where the output (target) is one of two possible values, like:
 
           ✅ Pass / ❌ Fail

           👍 Yes / 👎 No

           🔵 Class 0 / 🔴 Class 1


Despite its name, logistic regression is a classification algorithm, not a regression one.

### ⚙️ How Does It Work?

**Step 1: Linear Combination of Inputs**  

In mathematics, we model relationships between inputs and outputs. Logistic regression starts by computing a linear combination of the input features:

                                                z = w1x1 + w2x2  +⋯+ wnxn + b


Where:

      𝑥1 , 𝑥2 ,..., 𝑥𝑛  are the input features (like hours studied, number of attempts).

      w1 , w2 ,... , wn are the weights the model learns during training (they show how important each feature is).

      b is the bias term, similar to the y-intercept in a linear equation.

🔍 This is the same step used in linear regression, but logistic regression doesn’t stop here.

**✅ Step 2: Apply the Sigmoid Function**

Now we need to convert this linear output z (which can be any real number, even negative) into a probability between 0 and 1.

For that, logistic regression uses the sigmoid function:

                                                      σ(z) = 1 /  1 + e−z

This function always outputs a value between 0 and 1, no matter what the input is. That value represents the probability of the data point belonging to class 1.

**✅ Step 3: Make a Prediction**

Once we have the probability 𝜎(𝑧) we apply a threshold to classify:

                                       If σ(z) ≥ 0.5: Predict class 1

                                       If σ(z) < 0.5: Predict class 0

🔁 This threshold (default 0.5) can be changed if you want to make the model more or less sensitive.

### 🧪 Training (How the Model Learns)

During training, the model:

                       Initializes random weights and bias.

                       Uses the sigmoid function to make predictions on the training data.

                       Calculates how far off the predictions are using a loss function (usually log loss).

                       Uses gradient descent to adjust weights and bias to reduce the loss.

                       This process repeats until the model reaches good accuracy.
                       

### 🧠 Key Intuition:

Logistic regression doesn’t just give “yes” or “no”; it gives a probability and then classifies based on it.

It's simple, fast, and works well when your classes are linearly separable (can be separated by a straight line or hyperplane).


 

​
 

​



​
 
​

 


​
