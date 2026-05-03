# Trauma-Vis

**A web-based trauma phenotype visualization platform for precision trauma care.**

<img src="https://github.com/user-attachments/assets/7816daa4-8984-48e6-a22a-ec3a055c19fb" width="480"><br/>

Live application: [Trauma-Vis Shiny App](https://jotarotachino.shinyapps.io/TraumaApp250305/)<br/>
Repository README updated: 3 May 2026

Trauma-Vis is an online research platform for real-time identification and visualization of trauma phenotypes, integrated with conventional trauma prognostic models including ISS, RTS, TRISS, rSIG, and a phenotype-augmented TRISS complementary model.

## Citation
If you use Trauma-Vis in academic work, please cite this repository using GitHub's **Cite this repository** function and cite the related publications listed below. Citation metadata are provided in [`CITATION.cff`](CITATION.cff).

## Research contact
**Jotaro Tachino, MD, PhD**  
Department of Traumatology and Acute Critical Care Medicine, University of Osaka, Japan

Profiles: [researchmap](https://researchmap.jp/jotarotachino?lang=en) | [ORCID](https://orcid.org/0000-0002-0423-7713) | [PubMed bibliography](https://www.ncbi.nlm.nih.gov/myncbi/jotaro.tachino.1/bibliography/public/) | [Google Scholar search](https://scholar.google.com/scholar?q=%22Jotaro%20Tachino%22)

I am interested in advancing precision trauma care by integrating trauma phenotyping, prognostic modeling, treatment-effect heterogeneity analysis, causal inference, and trauma proteomics. Trauma-Vis was developed as part of this research program to translate trauma phenotype research into an accessible web-based platform for visualization, hypothesis generation, and collaborative research.

Research areas: precision trauma care, trauma phenotyping, treatment-effect heterogeneity, prognostic modeling, and trauma proteomics.

## Trauma phenotype
In previous research, eight trauma phenotypes were identified through cluster analysis of derivation cohort data from the Japan Trauma Data Bank (JTDB) from January 2013 to June 2015. The optimal number of clusters was determined using the average silhouette score and k-means method. After standardizing patient data, clustering was performed based on Euclidean distance using silhouette analysis, leading to the development of trauma phenotypes.<br/>

## Online platform
This online platform is a trauma analysis system developed using Shiny R that enables real-time identification and visualization of trauma phenotypes alongside traditional prognostic models. When new patient data is entered, it undergoes standardization followed by principal component analysis. The resulting principal component scores are used to calculate Euclidean distances between the new patient and derivation cohort patient data. The k-nearest neighbor method (k = 50) identifies the 50 most similar cases, and their cluster membership is visualized as pictograms. Abbreviated Injury Scale (AIS) scores are converted to dummy variables through one-hot encoding, and Uniform Manifold Approximation and Projection (UMAP) is applied for nonlinear dimensionality reduction, allowing visualization of cluster membership in low-dimensional space (displayed as "New" on the UMAP).
 <br/>
Users can input variables through side widgets to calculate traditional trauma scores (Injury Severity Score [ISS], Revised Trauma Score [RTS], and Trauma and Injury Severity Score [TRISS]) and the reverse shock index multiplied by the Glasgow Coma Scale score (rSIG). Additionally, they can calculate predicted survival rates based on a TRISS complementary model incorporating trauma phenotypes. This platform is an integrated system that implements traditional trauma outcome prediction models while providing real-time visualization of trauma phenotypes through pictograms and UMAP-based dimensionality reduction maps.<br/>
Research collaborators are granted permission to save input data as datasheets in the cloud. <br/>

## Reference
1) Tachino J., Matsumoto H., Sugihara F., Seno S., Okuzaki D., Kitamura T., Komukai S., Kido Y., Kojima T., Togami Y., Katayama Y., Nakagawa Y., Ogura H.: Development of clinical phenotypes and biological profiles via proteomic analysis of trauma patients. [Crit Care. 2022; 26:1:241.](https://ccforum.biomedcentral.com/articles/10.1186/s13054-022-04103-z)<br/>
2) Tachino J., Seno S., Matsumoto H., Kitamura T., Hirayama A., Nakao S., Katayama Y., Ogura H., Oda J.: Association between tranexamic acid administration and mortality based on the trauma phenotype: a retrospective analysis of a nationwide trauma registry in Japan. [Crit Care. 2024; 28:1:89.](https://ccforum.biomedcentral.com/articles/10.1186/s13054-024-04871-w)<br/>
3) Tachino J., Nakao S., Matsumoto H., Katayama Y., Kitamura T., Seno S., Oda J.: Approach to Optimizing Tranexamic Acid Use in Trauma: Potential Utilization of Trauma Phenotypes. [Thromb Haemost. 2026 online-ahead](https://www.thieme-connect.de/products/ejournals/abstract/10.1055/a-2806-3484)

## Legal Disclaimer and Terms of Use
### Purpose and Limitations
This application serves as a decision-support tool to assist in predicting outcomes for trauma patients. It is designed to complement, but never replace, clinical judgment. This system should be used exclusively as a decision-support aid in conjunction with professional medical assessment.
### Non-Medical Advice Disclaimer
This application does not constitute medical practice or provide specific medical advice, nor does the use of the application establish a doctor-patient relationship. For medical treatment or answers to personal questions, we strongly encourage you to consult with a qualified healthcare provider. For advice about your own care, please ask your doctor.
### Usage Agreement and Liability
You assume full responsibility for using this application, and you understand and agree that we are not responsible or liable for any claim, loss, or damage resulting from its use. While we strive to keep the information in the application as accurate as possible, we disclaim any warranty concerning its accuracy, timeliness, and completeness, and any other warranty, express or implied, including warranties of merchantability or fitness for a particular purpose. We do not warrant that access to the application will be error- or virus-free.
### Research Restrictions
As trauma phenotype research is still ongoing, users are requested to refrain from conducting clinical research or publishing papers using this platform without proper authorization.
### Acceptance
By using this application, you acknowledge that you have read, understood, and agreed to these terms and conditions.
