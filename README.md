## JMeter Performance Testing Results After Refactor

### All-Student-Name Endpoint

| Before | After |
|--------|-------|
| ![img_4.png](img_4.png) | ![img_5.png](img_5.png) |
| ![img_6.png](img_6.png) | ![img_7.png](img_7.png) |

### Highest-GPA Endpoint

| Before | After |
|--------|-------|
| ![img_8.png](img_8.png) | ![img_9.png](img_9.png) |
| ![img_10.png](img_10.png) | ![img_11.png](img_11.png) |

### Test Result Logs: All-Student-Name

| Before | After |
|--------|-------|
| ![img.png](img.png) | ![img_2.png](img_2.png) |

### Test Result Logs: Highest-GPA

| Before | After |
|--------|-------|
| ![img_1.png](img_1.png) | ![img_3.png](img_3.png) |

### Get All Students and Courses

| Before | After |
|--------|-------|
| ![image](https://github.com/user-attachments/assets/0819e2ff-df36-4009-9c45-6f844cc82f11) | ![image](https://github.com/user-attachments/assets/5c717c86-cefd-46d2-adca-7f385cd22dab) |

#### **Conclusion:**
![image](https://github.com/user-attachments/assets/7e58663f-594b-423a-87c4-0e5a8ae853a9)

### Highest GPA

| Before | After |
|--------|-------|
| ![image](https://github.com/user-attachments/assets/fd3fa7c4-3c9e-4b16-bdd6-cb876e82cf11) | ![image](https://github.com/user-attachments/assets/1e3a11ef-f7dd-4c65-b8a3-84249735a900) |

#### **Conclusion:**
![image](https://github.com/user-attachments/assets/f7331e68-8476-4279-a445-68370d2e429c)

### Find All Students

| Before | After |
|--------|-------|
| ![image](https://github.com/user-attachments/assets/83f188c3-7e61-4e5d-ac57-d2ffd2d05fe5) | ![image](https://github.com/user-attachments/assets/7aa39611-0d3f-49ab-8564-fe6f9720f0f8) |

#### **Conclusion:**
![image](https://github.com/user-attachments/assets/7a908526-8ad1-48bc-aa32-3b795c65cb67)

## JMeter After Refactor: **All-Student Endpoint**

| Before | After |
|--------|-------|
| ![image](https://github.com/user-attachments/assets/4d0e9bd5-85f2-4a94-bd70-1f46f3c7bab9) | ![image](https://github.com/user-attachments/assets/7dd33826-7515-449c-9e19-bd1e776a3733) |
| ![image](https://github.com/user-attachments/assets/9b7e43e0-0c08-4a2c-bb1f-41a1eeb8127e) | ![image](https://github.com/user-attachments/assets/5d77aeb2-6f83-46ec-9797-c37bf37c1fa1) |

## JMeter After Refactor: **All-Student-Name Endpoint**

| Before | After |
|--------|-------|
| ![image](https://github.com/user-attachments/assets/c4b854e0-e58b-48b2-bbeb-d14ec61224df) | ![image](https://github.com/user-attachments/assets/42af39eb-5ac5-44e5-a7ae-99f52cbe81b3) |
| ![image](https://github.com/user-attachments/assets/bf12d468-4070-4759-bd1c-fc197d094b28) | ![image](https://github.com/user-attachments/assets/6231e3be-025f-4bff-b2d7-b3a58a632bd3) |

## JMeter After Refactor: **Highest-GPA Endpoint**

| Before | After |
|--------|-------|
| ![image](https://github.com/user-attachments/assets/552fd314-3387-4165-8031-4f1a1d77573d) | ![image](https://github.com/user-attachments/assets/a3248f94-a412-4f8f-9c1f-0b5be8bf5e9d) |
| ![image](https://github.com/user-attachments/assets/b833bf13-5542-4b06-9724-af4c172e9f7f) | ![image](https://github.com/user-attachments/assets/41b1a673-5779-4024-8d29-e4c30668dc11) |


### Reflection
#### What is the difference between the approach of performance testing with JMeter and profiling with IntelliJ Profiler in the context of optimizing application performance?
Load testing and performance testing are what JMeter is mainly used for, and it accomplishes these tasks by simulating a number of users and then analyzing the response times. In contrast, the IntelliJ Profiler is not a tool for overall system assessment, but rather for doing code-level profiling. It helps you determine which parts of your code are consuming CPU time, using excessive memory, or otherwise not operating efficiently. 

#### How does the profiling process help you in identifying and understanding the weak points in your application?
Profiling helps by providing live insights on CPU and memory usage, allowing us to identify performance bottlenecks, inefficient loops, etc. By analyzing method execution times, we can determine which parts of the code slow down the application and optimize accordingly.

#### Do you think IntelliJ Profiler is effective in assisting you to analyze and identify bottlenecks in your application code?
Yeah, it tells me which parts of my code are running too slow and what methods I have to fix to increase the overall performance of my application. I also get to see the specific difference in CPU time needed to run the application before and after code revisions now, which helps a lot with development.

#### What are the main challenges you face when conducting performance testing and profiling, and how do you overcome these challenges?
For me it was pretty hard to grasp the concept of performance testing and profiling at first, as there were so many listeners to check out and so many types of insights and graphs that could be provided by Jmeter and IntelliJ Profiler. Over time, I'm learning how to better understand these performance reports by asking my friends and also using resources on the Internet.

#### What are the main benefits you gain from using IntelliJ Profiler for profiling your application code?
I think it's very convenient to have a profiler built into IntelliJ as it means I don't have to do external set-ups with third party applications. The profiler also helps me find out where the bottlenecks of my application are at. It also aids me in evaluating the performance before and after I attempt to fix these bottlenecks.

#### How do you handle situations where the results from profiling with IntelliJ Profiler are not entirely consistent with findings from performance testing using JMeter?
When test results from a profiler differ from JMeter findings, I look first at the test environments. I check to see if any differences in configuration, deployment, or even underlying hardware could have caused the profiler to produce inaccurate results. I also closely inspect the dataset being used in the tests. 

#### What strategies do you implement in optimizing application code after analyzing results from performance testing and profiling? How do you ensure the changes you make do not affect the application's functionality?
After performance testing and profiling, I find out which method and functions are causing a bottleneck. Then, I try to make those methods and functions more efficient by using streams and appropriate database queries. To ensure changes don’t affect functionality, I rely on unit tests and integration tests.








