# RAP_COI_Testing_Talk

<img src="https://github.com/mamonu/RAP_COI_Testing_Talk/raw/master/RAPz.jpg" data-canonical-src="https://github.com/mamonu/RAP_COI_Testing_Talk/raw/master/RAPz.jpg" width="200" height="200" />


A short talk about testing and how it relates to  RAP (Reproducible Analytical Pipelines)


Covering :

- [x] What to test?
- [x] Manual Testing
- [x] Coverage
- [x] Automated testing 
- [x] Property based testing
- [x] Mutation Testing
- [x] Integration Testing
- [x] End2End Testing
- [x] Continuous Integration (CI)
- [x] Documentation (autodoc)
- [x] Memes


It has a Python slant but I tried to include R implementations where availiable. 
But what I really wanted to talk about was the concepts.


It was presented on  28th/May/2019 at the Reproducible Analytical Pipelines Community of Interest gathering at ONS in London

---

Here are some blog posts I wrote related to the subjects above:

* Introductory material about testing covered [here](https://mamonu.github.io/Testing/])
* Talking about pytest, some example simple tests with it and calculating coverage [here](https://mamonu.github.io/testing_coverage/)
* Talking about property based testing in more detail and some examples [here](https://mamonu.github.io/Property-Based-Testing/)

---
---

##### TLDR concepts

Essential:



- Unit testing (basic anecdote-based testing)

  Anecdote based testing. Test your functions with specific inputs and expect specific outputs

- Unit testing (automatic with parameterization)

   Same as above but include more than one set of inputs and outputs. The more the merrier. 
   Parametrized tests will be called multiple times, each time executing the set of dependent tests. 
   Test functions usually do not need to be aware of their re-running.

- Integration testing (less tests that unit tests)  

  Testing performed to expose defects in the interfaces and in the interactions between pipeline steps.

- End to End Testing (even less tests but to test whole pipeline)

  There may still be emergent issues when the whole pipeline is used together hence E2E testing needed


Nice to Have:

- Continuous Integration

  Every time someone tries to integrate / add code to a codebase the following things need to happen:
  
  * merge new code with old code in a test environment
  * run a series of tests (many unit tests,less integration tests,few e2e tests)
  * if none of the tests is throwing an error then code is accepted to repo (or at least this is the point that perhaps code review can take place
  

- Coverage metrics (useful metric but not end-all-be-all)

- Property based unit tests 

- Mutation unit tests


---
---

##### TLDR links



- Some Books of interest (perhaps to find in local or organisation library) :

    
    https://www.goodreads.com/book/show/25819310-software-testing
  
    https://www.oreilly.com/library/view/python-testing-with/9781680502848/
  

---

- Blog Posts


    https://martinfowler.com/articles/practical-test-pyramid.html

    https://medium.com/homeaway-tech-blog/write-better-python-with-hypothesis-5b31ac268b69
    
    https://blog.codecentric.de/en/2016/01/mutation-testing-watching-watchmen/
    
 
 ---
 
-   Documentation from selected modules   

    
    https://hypothesis.works/articles/
  
    https://docs.pytest.org/en/latest/  
    
    https://nox.readthedocs.io/en/stable/


---

- Course


   Great course covering the spectrum of tools from the R side of things:
  
  
  
    https://www.udemy.com/reproducible-analytical-pipelines/

---


- Covered / useful Python modules: 


  py.test : https://github.com/pytest-dev/pytest *
  
  mutpy : https://github.com/mutpy/mutpy
  
  mutmut : https://github.com/boxed/mutmut
  
  cosmic_ray  : https://github.com/sixty-north/cosmic-ray  *
  
  hypothesis : https://github.com/HypothesisWorks/hypothesis  *
  
  tox : https://github.com/tox-dev/tox
  
  nox : https://github.com/theacodes/nox
  
  cookiecutter: https://github.com/audreyr/cookiecutter
  
  pyjanitor : https://github.com/ericmjl/pyjanitor *
  
  sphinx-doc : http://www.sphinx-doc.org/en/master/


*recomended


---

- Covered / useful R modules: 

    Hedgehog: https://github.com/hedgehogqa/r-hedgehog *
    
    cookiecutter-r : https://github.com/bdcaf/cookiecutter-r-data-analysis

*recomended

---

- Article : When RAP processes are not there...

  https://www.bbc.co.uk/news/magazine-22223190



