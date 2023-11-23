* Frameworks and language used
  
    * Springboot and java
* Data flow
  1. Controller
     * AdminController
     * UserController
  2. Services
     * AdminService
     * AuthenticationService
     * CommentService
     * FollowService
     * LikeService
     * PostService
     * UserService
  3. Repository
     * IAdminRepo
     * IAuthenticationRepo
     * ICommentRepo
     * IFollowRepo
     * ILikeRepo
     * IPostRepo
     * IUserRepo
  4. Model
     * Admin
     * AuthenticationToken
     * Comment
     * Follow
     * Like
     * Post
     * User
  5. Database Used
     * MySQL database

* # Project Summary
   In this project we created InstaBackend basic design project and used mysql database to store the data. We create different type of mapping.
  It follows MVC-architecture.In this application, I have also provided some of the validators on the field values and if a user puts invalid details in response,
  it will handle exception and will revert with Http Status code 400 as a BAD_REQUEST.
  The pupose of the project is, If user wants to create his account on Instagram then he has to be sign up and Only sign up user can able to sign in.
  The extra model is for authentication of user who has done signUp / signIn or not. Every User has unique email address and we get authorized through that email which generating token to making user accessible to that app.
  For posing the data, we are performing crud operations on it with the help of endpoints like @GetMapping to get all the information of the Model, @PostMapping to create a Model Information using the attributes.
