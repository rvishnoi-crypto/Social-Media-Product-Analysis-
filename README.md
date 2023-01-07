# Social-Media-Product-Analysis-

Online controlled experiments, digital versions of randomized controlled trials, seek to use user-generated data to test and improve internet-based products and services. Informally referred to as A/B tests, these experiments are an indispensable tool for major technology companies when it comes to maximizing revenue and optimizing the user experience. Industry giants run hundreds of experiments on millions of users every day, testing changes to websites, services, and installed software; desktop and mobile devices; front- and back-end product features; personalization and recommendations; and monetization strategies.

In this project will consider a totally hypothetical A/B test at the social media site, Chirper. Chirper is conducting an upgrade of their server system; Old_Serv had some apparent ‘bloatware’ that New_Serv has removed. Interest lies in comparing the page load times (PLT) associated with the old and new server systems. Ideally, New_Serv would be associated with faster (i.e., smaller) page load times.

It’s important to recognize that page load time distributions tend to be right-skewed and optimizing for average page load time is not as useful as optimizing tail performance; since the user experience associated with high page load times is negative, it is better to minimize worst case scenarios; minimizing typical page load times is not sufficient. As such, interest lies in comparing Qold(0.95) and Qnew(0.95), the 95th percentiles (i.e., the 0.95 quantiles) of the PLT distributions in the two server settings. While many two- sample hypothesis tests exist for comparing quantiles, we use a randomization test one

While the team hopes the new server setup performs better in this respect, interest initially lies in determining whether there is a difference at all between Qold(0.95) and Qnew(0.95). To determine this, the team runs an experiment in which 1000 randomly selected Chirper page requests are randomly assigned either the old (Nold = 500) or the new (Nnew = 500) server system. The load time (in seconds) for each load request is recorded. These data are available in the file pageload.csv.
