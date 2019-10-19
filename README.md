# notthatDDT
DDT: Database of dynamics trajectories

We will establish a website that contains videos of representative trajectories for a variety of organic reactions. We will focus on reactions taught in undergraduate organic chemistry courses. The goal is to provide instructors with videos they can show students of molecules vibrating in meaningful ways while reacting. 

This will be a long term project involving undergrads/new grads who are interested in dynamics project.

See separate repository that stores the website. 

###Table of Content:
***
1. [General info](#General_info)
2. [How to run dynamics](#How_to_run_dynamics)
3. [How to generate movies](#How_to_generate_movies)

<a name="General_info"><a/>
#### 1. General_info
To accomplish one organic system for this project, you need to:
-  Find TSS of the reaction with gaussian. With proper functional and basis set. Example as follow:
```
%nprocshared=8
%mem=16GB
%chk=sn2Cl_ts.chk
# opt=(calcfc,ts,noeigen) freq b3lyp/6-31g(d) EmpiricalDispersion=GD3 scf=xqc
```

-  Use the TSS above to do dynamics and get trajectories. Detail see second section "How to run dynamics".

- Calculate reactant and product structure. Calculate IRCs on both direction.

-  Generate movies for both IRC and dynamics trajctories.


<a name="How_to_run_dynamics"><a/>
#### 2. How to run dynamics
See dynamics_tutorial_files folder

<a name="How_to_generate_movies"><a/>
#### 2. How to generate movies
See make_movie_tutorial_files folder
