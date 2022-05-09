# MedRed_Reproducible

Reproducing models for suggesting diagnoses based on social media posts and comments, from

>Sanja Scepanovic, Enrique Martin-Lopez, Daniele Quercia, and Khan Baykaner. 2020. Extracting medical entities from social media. In Proceedings of the ACM Conference on Health, Inference, and Learning (CHIL '20). Association for Computing Machinery, New York, NY, USA, 170–181. DOI:[https://doi.org/10.1145/3368555.3384467](https://doi.org/10.1145/3368555.3384467)

## Execution

Simply follow the notebooks in the code folder. Paths in the Constants labeled cells may need to be adjusted depending on your environment.

Start with data preparation: `medred_prep.ipynb`, `cadec_prep.ipynb`, and `micromed_prep.ipynb`.

Then proceed to `NER_prep.ipynb` set up the datasets for Med-DL. Once this is completed, train with `train.ipynb`. Test sets can be evaluated with `eval.ipynb`.

Validation with predictors can be done using `reddit_validation_embed.ipynb`, `reddit_feature_gen.ipynb`, and `reddit_predictions.ipynb` in that order. Post correlations are also processed there.

# Results

Results are available in the corresponding notebooks.

# Dependencies

For dependencies, see `environment.yml`.

# Notes

Models and data are not included here. The datasets are available at:

- MicroMed: https://github.com/IBMMRL/medinfo2015
- CADEC: https://data.csiro.au/collection/csiro:10948?q=CADEC&_st=keyword&_str=1&_si=1
- MedRed and Reddit 500k: https://figshare.com/articles/dataset/MedRed/12039609/1

# References

Sanja Šćepanović, Enrique Martin-Lopez, Daniele Quercia, and Khan Baykaner. 2020. Extracting medical entities from social media. In Proceedings of the ACM Conference on Health, Inference, and Learning (CHIL ’20). Association for Computing Machinery, New York, NY, USA, 170–181. https://doi.org/10.1145/3368555.3384467

Sanja Šćepanović, Enrique Martín-López and Daniele Quercia (2020): MedRed. Figshare. Dataset. https://doi.org/10.6084/m9.figshare.12039609.v1

Jimeno-Yepes, A., MacKinlay, A.D., Han, B., & Chen, Q. (2015). Identifying Diseases, Drugs, and Symptoms in Twitter. Studies in health technology and informatics, 216, 643-7 .

Jimeno-Yepes, A., MacKinlay A.. (2016). NER for medical entities in Twitter using sequence to sequence neural networks. In Proceedings of the Australasian Language Technology Association Workshop. 138–142.

Karimi, S., Metke-Jimenez, A., Kemp, M., & Wang, C. (2015). Cadec: A corpus of adverse drug event annotations. Journal of Biomedical Informatics, 55, 73–81. https://doi.org/10.1016/j.jbi.2015.03.010

Karimi, Sarvnaz; Metke Jimenez, Alejandro; Kemp, Madonna; Wang, Chen (2015): CADEC. v3. CSIRO. Data Collection. https://doi.org/10.4225/08/570FB102BDAD2

Leaman R, Lu Z (2016) "TaggerOne: Joint Named Entity Recognition and Normalization with Semi-Markov Models", Bioinformatics, in press.

Tutubalina, E., & Nikolenko, S. (2017). Combination of Deep Recurrent Neural Networks and Conditional Random Fields for Extracting Adverse Drug Reactions from User Reviews. Journal of healthcare engineering, 2017, 9451342. https://doi.org/10.1155/2017/9451342