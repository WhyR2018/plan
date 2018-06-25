# Machine-learning and R for purposes of plastic surgery -- classification and attractiveness evaluation of facial emotions

[Lubomír	Štěpánek,	First Faculty of Medicine, Charles University & Faculty of Biomedical Engineering, Czech Technical University in Prague]()

## Description

Many current studies come to a conclusion that facial attractiveness perception is data-based and irrespective of the perceiver. However, the ways how to analyse associations between facial geometric image data and its visual impact always exceeded the power of classical statistical methods. In this study, we have applied machine-learning methods to identify geometric features of a face associated with an increase of facial attractiveness after undergoing rhinoplasty, a plastic surgery procedure for correcting the form and functions of a nose. Furthermore, current plastic surgery deals with aesthetic indications such as an improvement of the attractiveness of a smile or other facial emotions, hence we explored how accurate classification of faces into sets of facial emotions and their facial manifestations is, since categorization of human faces into somatotypes should take into consideration the fact that total face impression is also dependent on expressed facial emotion.

Both profile and portrait facial image data were collected for each patient, processed, landmarked and analysed using R language. Facial attractiveness was measured using Likert scale by a board of independent observers. Multivariate linear regression was performed to select predictors increasing facial attractiveness after undergoing rhinoplasty. The sets of used facial emotions and other facial manifestation originate from Ekman-Friesen FACS scale but was improved substantially. Bayesian naive classifiers using e1071 package, regression trees (CART) via tree and rpart packages and, finally, neural networks by neural net package were learned to allow assigning a new face image data into one of the facial emotions.

Enlargements of both a nasolabial and nasofrontal angle within rhinoplasty were determined as statistically significant predictors increasing facial attractiveness. Neural networks manifested the highest predictive accuracy of a new face categorization into facial emotions. Geometrical shape of a mouth, then eyebrows and finally eyes affect in descending order the (quality of) classified emotion, as was identified using decision trees.

We performed machine-learning analyses to point out which facial geometric features, based on large data evidence, affect facial attractiveness the most, and therefore should preferentially be treated within plastic surgeries. Additionally, the classification indicated new possible facial somatotypes based both on facial geometry and expressed emotions, and suggested which facial features determine the final assignment into one of the classes of emotions the most.

References:
-- Pavel Kasal, Patrik Fiala, Lubomír Štěpánek, et al. “Application of Image Analysis for Clinical Evaluation of Facial Structures”. In: Medsoft 2015 (2015), pp. 64–70. URL: http://www.creativeconnections.cz/medsoft/2015/Medsoft_2015_kasal.pdf
