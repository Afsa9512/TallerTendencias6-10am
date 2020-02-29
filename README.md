
# Machine Learning
The advent of ***big data***, cloud computing, and machine learning are revolutionizing how many professionals approach their work. These technologies offer exciting new ways for engineers to tackle real-world challenges. But with little exposure to these new computational methods, engineers lacking data science or *experience* in modern **computational methods** might feel left behind.
### Current Uses of AI:

Nombre|Descripcion
---|---
Email filtering | Email services use artificial intelligence to filter incoming emails. Users can train their spam filters by marking emails as “spam”.
Personalization | Online services use artificial intelligence to personalize your experience. Services, like Amazon or Netflix, “learn” from your previous purchases and the purchases of other users in order to recommend relevant content for you.
* Porción de código Python
~~~
while not is_convergence(a, b, a_old, b_old, convergence) \
            and it_counter < iterations:
        a_old = a
        b_old = b
        sum_a, sum_b = (0,) * 2
        for i, r in samples.iterrows():
            h = get_hipotesis(a_old, b_old, r['Tiempo'])
            diff = get_diff(h, r['Calorias'])
            sum_a += diff * r['Tiempo']
            sum_b += diff
        a = a_old - ((ALPHA / len(samples)) * sum_a)
        b = b_old - ((ALPHA / len(samples)) * sum_b)

        it_counter += 1
        print_iteration_status(it_counter, a, b, get_error(samples, a, b))

    print_results(a, b, get_error(samples, a, b))
    plot_results(samples['Tiempo'].tolist(), samples['Calorias'].tolist(), a, b)
~~~

> Cita
