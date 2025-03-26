# MyPaper
Some supplementary descriptions and experiments for my paper

We selected CAMOUFLaG-Base (C-Base), and Face Anonymization Made Simple (FAMS) which are both the latest diffusion-based methods. We conducted tests on the CelebA-HQ dataset, which is shared by all three papers. We use FID for image quality, re-identification rate for anonymization, pose and expression distances for geometric attributes preservation, and the classification accuracy rates of age, gender, and make-up for semantically strongly correlated attributes preservation. The results show that C-Base can achieve excellent preservation of semantically strongly correlated attributes, but it is insufficient in terms of anonymization, the preservation of geometric attributes, and image quality. FAMS can achieve good preservation of geometric attributes, yet it is unsatisfactory in semantically strongly correlated attributes preservation. Our method achieves the best performance in terms of FID, expression distance, as well as the preservation of age and gender attributes. Given that our model was not trained on this dataset while the other two models were, this also demonstrates its excellent robustness.

\begin{table}[t]
\centering
\caption{Comparison with the latent diffusion-based methods.}
\label{tab:table}
    \resizebox{0.48\textwidth}{!}{
    \large
    \begin{tabular}{*{10}{c}}
        \toprule
       Methods & FID ↓ & ReID ↓ & pose ↓ &  expression ↓ & age ↑&  gender ↑&  makeup ↑ \\
        \midrule
        C-Base & 34.33 & 0.25 & 8.61 & 0.68 & \underline{0.89} & \textbf{0.99} & \textbf{0.89} \\
        FAMS & \underline{10.93} & \textbf{0.03} & \textbf{6.58} & \underline{0.56} & 0.77 & \underline{0.61} & 0.56 \\
        Ours & \textbf{7.40} & \underline{0.05} & \underline{8.36} & \textbf{0.54} & \textbf{0.90} & \textbf{0.99} & \underline{0.82} \\
        \bottomrule
    \end{tabular}
    }
    \vspace{-1em}
\end{table}
