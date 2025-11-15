# Visual-Illusion-NeuroAI
1. What This Project Is About

Humans sometimes see things that are not actually true — that’s what we call visual illusions.

For example, in the Müller–Lyer illusion, two lines that are exactly the same length appear different because of the arrowheads at their ends.

I wanted to test a simple question:

Do computer vision models get fooled by this illusion the same way humans do?

To answer this, I used a pretrained deep learning model (MobileNetV2) and studied how its internal activations change when it looks at illusion vs non-illusion images.

This connects to NeuroAI, where researchers compare human perception and artificial neural networks.

⸻
 2. What Images I Used

I generated two types of images:
	1.	Illusion Image
	•	shows the Müller–Lyer illusion
	•	lines look different but are actually identical
	2.	Control Image
	•	just a plain straight line
	•	no arrowheads, no illusion

This helps in comparing how the model behaves in both situations.

⸻
 3. How I Tested the CNN

I used MobileNetV2, a convolutional neural network trained on millions of images.

I passed both images (illusion and control) through an early layer of the model, which acts like the model’s “early visual cortex.”

Then I measured:
 How much the internal activations of the network change between the two images.

If the difference is large → the model is sensitive to the illusion.
If the difference is small → the model is not very fooled.

⸻
 4. What the Results Showed
	•	The difference in activations between illusion and control was around 0.10.
	•	This is not zero, so the model does react differently.
	•	But it is not very large, so the model is not strongly fooled.

✔ The CNN detects some changes

✘ But it does not “fall for” the illusion like humans do

This is actually consistent with real research:
CNNs don’t have the same top-down perception and cognitive biases that make humans experience visual illusions strongly.

⸻
 5. Visualizations

I also plotted:
	•	The illusion image
	•	The control image
	•	The CNN’s activation map
	•	A bar chart showing the activation difference

These visualizations make it easy to understand how the model processes the image internally.

⸻
 6. Why This Project Is Useful

This small project demonstrates:
	•	understanding of computer vision
	•	experience with deep learning models
	•	ability to analyze neural activations
	•	interest in NeuroAI (an important area at University of Amsterdam)
	•	skills in experimentation and interpretation

It also shows how AI models and human brains differ in the way they perceive the world.
