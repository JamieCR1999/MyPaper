# MyPaper
Some supplementary descriptions and experiments for my paper

We selected CAMOUFLaG-Base (C-Base), and Face Anonymization Made Simple (FAMS) which are both the latest diffusion-based methods. We conducted tests on the CelebA-HQ dataset, which is shared by all three papers. We use FID for image quality, re-identification rate for anonymization, pose and expression distances for geometric attributes preservation, and the classification accuracy rates of age, gender, and make-up for semantically strongly correlated attributes preservation. The results show that C-Base can achieve excellent preservation of semantically strongly correlated attributes, but it is insufficient in terms of anonymization, the preservation of geometric attributes, and image quality. FAMS can achieve good preservation of geometric attributes, yet it is unsatisfactory in semantically strongly correlated attributes preservation. Our method achieves the best performance in terms of FID, expression distance, as well as the preservation of age and gender attributes. Given that our model was not trained on this dataset while the other two models were, this also demonstrates its excellent robustness.

![image](https://github.com/user-attachments/assets/5e0bbe7f-bd36-4a41-bbb6-90a49a7a502a)

