# Recommendation Systems
## Movie Recommendations

<details>
        <summary>Context</summary>
        <br>
        <p style='text-align:justify;'>
        Online streaming platforms like Netflix have plenty of movies in their repositories and if we can build a recommendation system to recommend relevant movies           to users based on their historical interactions, this would improve customer satisfaction and hence improve revenue. The techniques that we will learn here             will not only be limited to movies, it can be any item for which you want to build a recommendation system. For this case study, you can find the dataset               <a href=https://www.kaggle.com/rounakbanik/the-movies-dataset>here</a>.
        </p>
</details>

<details>
        <summary>Objective</summary>
        <br>
        <p style='text-align:justify;'>
          In this project we will be building various recommendation systems: 
        <ul>
        <li> Knowledge/Rank based recommendation system</li>
        <li> Similarity-Based Collaborative filtering</li>
        <li> Matrix Factorization Based Collaborative Filtering</li>
        </ul>
based on the **ratings** dataset
        </p>
</details>

<details>
        <summary>Data Dictionary</summary>
        <br>
        <p style='text-align:justify;'>
             The dataset has the following information:   
        <ul>
                <li><code>userId</code></li>
                <li><code>movieId</code></li>
                <li><code>rating</code></li>
                <li><code>timestamp</code></li>   
        </ul>
        </p>
</details>

<details>
        <summary>Summary of key findings & insights</summary>
        <br>
        <p style='text-align:justify;'>
                In conclusion:
        <ul>
                <li>User-based collaborative model is slightly better than Item-based Collaborative model. User based RMSE value is 0.9672 while the "Item based" model's RMSE is 1.0032. Clearly, tuned Collaborative Filtering Models have performed better than baseline model and the user-item based tuned model is performing better having rmse of 0.943.</li>
                <li>The Collaborative Models use the user-item-ratings data to find similarities and make predictions rather than just predicting a random rating                       based on the distribution of the data. This could a reason why the Collaborative filtering performed well.</li>
                <li>Collaborative Filtering searches for neighbors based on similarity of item (example) preferences and recommend items that those neighbors                           interacted while Matrix factorization works by decomposing the user-item matrix into the product of two lower dimensionality rectangular                             matrices. </li>
                <li>RMSE for Matrix Factorization (0.9064) is better than the Collaborative Filtering Models (~1.00). Tuning SVD matrix factorization model improved                     the base line SVD with RMSE 0f 0.895. Matrix Factorization has lower RMSE due to the reason that it assumes that both items and users are                           present in some low dimensional space describing their properties and recommend a item based on its proximity to the user in the latent space.                       Implying it accounts for latent factors as well.</li>    
        </p>
</details>
