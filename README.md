<h2> Hi, I'm Alexandr Korikov AKA air2921 <img src="https://media.giphy.com/media/mGcNjsfWAjY5AEZNw6/giphy.gif" width="50"></h2>
<p><em>👀 I’m interested in WEB development via ASP.NET Core and Reactjs.
<p><em>👯 I’m looking to collaborate on Frontend developers on Reactjs, Angular, or Vue.
<p><em>📫 Reach me via <a href="https://t.me/air2921">telegram</a><img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExZmVnMWFpYTF3MTBpNnhqMjlia2lrcmVkYThnbGw4NHJ5YmpuYm1vaSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/wlR4kWTnwEyY8RwHKM/giphy.gif" width="30"> 

```cs
[HttpGet("{username}")]
public async Task<IActionResult> GetUser([FromRoute] string username)
{
    var userTask = _userRepository.GetByFilter(query => query.Where(u => u.username.Equals(username)));

    var myStack = new
    {
        languages = new string[] { "C#", "linq", "TypeScript", "html5", "css3" },
        tools = new string[] { "RESTApi/JSONApi", "Swagger", "Postman", "SignalR" },
        frameworks = new
        {
            backend = new string[] { "ASP.NET Core Web API", "ASP.NET Core MVC" },
            frontend = new string[] { "React.js" }
        },
        db = new
        {
            sql = new string[] { "PostgreSQL", "MS SQL Server" },
            noSql = new string[] { "Redis", "MongoDb" },
            orm = new string[] { "Entity Framework Core" }
        }
    };

    var user = await userTask;
    var social = new
    {
        name = user.name, // Alexandr Korikov
        username = user.username, // air2921
        gmail = user.email, // StewieSolden147@gmail.com
        telegram = user.telegram // https://t.me/air2921
    };

    return StatusCode(200, new { social, myStack });
}
```
