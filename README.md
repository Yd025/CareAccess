# Access to Care: Identifying Subgroups at Risk of Falling Through the Cracks

DubsTech Datathon 2026 | Adelin Ma

For this year's datathon, I chose the Access to Care pathway. Care access is something I think about all the time. I have been involved in various activities to boost accessibility in elder care specifically—from a six-month internship as a TechCare intern at a nonprofit for the elderly to working at a stroke ward in a community hospital. My recent efforts have focused on building accessible, customisable workout apps for people with limited mobility. I also speak with many people who fall through the cracks in the world. Care is not one-size-fits-all: different barriers and circumstances affect different groups, and the same person can slip through for different reasons depending on how we look at the problem.

With that in mind, I wanted to use three ML approaches—K-Means Clustering, Linear Regression, and a simple Deep Learning (MLP) model—to flag subgroups most at risk of poor access to care. I compared which subgroups each method identified and reported accuracy (MSE, R², silhouette) to see which model worked best and which groups to prioritize.

The data came from NHIS Adult Summary Health Statistics (CDC); I focused on access-to-care topics (delayed care, unmet care due to cost, uninsured). I felt that different methods answered different questions—clustering found who looked like the worst-off group, while regression found who was predicted to have the worst access—so the same population could "fall through the cracks" for different reasons depending on which lens I used.

## Software used

- **Python 3**
- **pandas** — data loading and manipulation
- **NumPy** — numerical operations
- **scikit-learn** — preprocessing (StandardScaler), K-Means clustering, Linear Regression, MLP regressor, and metrics (MSE, R², Silhouette score)
- **Seaborn** — correlation heatmap and visualizations
- **Matplotlib** — plotting
- **Jupyter** — notebook environment
