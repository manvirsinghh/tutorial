# Social Module in Frappe

The **Social Module** in Frappe is a feature set that enhances the user experience by providing social interaction tools within the Frappe framework. It is designed to enable communication, collaboration, and engagement among users of the platform. It includes features like activity tracking, user interaction through comments, notifications, and the management of gamified elements like energy points and user levels. This module is useful for applications that require social components such as feedback systems, discussions, activity tracking, and user engagement.

![image](https://github.com/user-attachments/assets/ca924fea-5870-4ba1-90ac-a8b32d85fcd1)

## Key Doctypes

### 1. Review Level

- **Purpose**: The Review Level doctype is used to define the different levels or ranks a user can achieve based on their activities or energy points.
- **Example Use Case**: You might have different levels like "Beginner", "Intermediate", and "Expert" based on the points accumulated.
- **Key Fields**: Typically, fields like Level Name, Points Range, and Level Description are used to define the criteria for each level.

#### Example:

- **Beginner**: 0 to 100 points
- **Intermediate**: 101 to 500 points
- **Expert**: 501 and above points

---

### 2. Energy Point Log

- **Purpose**: This doctype records all the actions or events that lead to a user earning energy points. It keeps a history of all the energy points that have been earned.
- **Example Use Case**: Whenever a user performs a certain action (e.g., completing a task, providing feedback, making a post), points are recorded in the Energy Point Log.
- **Key Fields**: Typically, fields like User, Points Earned, Action Type, Date/Time, and Description are used.

#### Example:

- **User**: John Doe
- **Points Earned**: 10
- **Action Type**: Completed a task
- **Description**: Earned 10 points for completing Task #123.

---

### 3. Energy Point Settings

- **Purpose**: This doctype is used to configure and manage the rules around how energy points are awarded. It defines the settings that affect how points are distributed for certain actions or behaviors.
- **Example Use Case**: You can set rules on how many points should be awarded for specific actions like commenting, completing tasks, or making a post.
- **Key Fields**: Fields such as Action Type, Points Awarded, Active (if the rule is active or inactive), and other configuration settings.

#### Example:

- **Action Type**: Completing a task
- **Points Awarded**: 10 points
- **Active**: Yes (This rule is active and will award points).

---

### 4. Energy Point Rule

- **Purpose**: This doctype defines the specific rules that govern how energy points are awarded to users. It sets the criteria and logic for earning points.
- **Example Use Case**: The Energy Point Rule might specify that users get 5 points for every comment they make or 20 points for each post.
- **Key Fields**: Fields such as Rule Name, Action, Points Awarded, Condition (optional), and Active.

#### Example:

- **Rule Name**: Commenting Rule
- **Action**: Comment
- **Points Awarded**: 5 points
- **Condition**: Only valid if the comment is more than 20 words long
- **Active**: Yes

---

## How These Doctypes Work Together

- **Energy Point Settings** define the basic configuration, like how many points are awarded for specific actions.
- **Energy Point Rule** is where the detailed rules are set up (e.g., 10 points for completing a task, 5 points for posting).
- **Energy Point Log** tracks the actual points users earn based on actions they take (e.g., comments, posts).
- **Review Level** is used to categorize users into different levels based on their accumulated energy points, incentivizing users to take actions that increase their points.

---

## Example Use Case

Let’s say we are running a social platform where users can complete tasks, comment on posts, and participate in discussions. Here’s how it works:

- **Energy Point Settings**:  
  We configure the system to give 10 points for completing a task and 5 points for each comment.

- **Energy Point Rule**:  
  We create a rule that says "Commenting on a post gives 5 points" and "Completing a task gives 10 points."

- **Energy Point Log**:  
  Whenever a user completes a task or comments on a post, the system records that in the Energy Point Log, tracking who did what and how many points they earned.

- **Review Level**:  
  After a user accumulates enough points, they move to the next Review Level, like from "Beginner" (0-100 points) to "Intermediate" (101-500 points).
