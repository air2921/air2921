<h2> Hi, I'm Alexandr Korikov AKA air2921 <img src="https://media.giphy.com/media/mGcNjsfWAjY5AEZNw6/giphy.gif" width="50"></h2>
<p>👀 I’m interested in WEB development via ASP.NET Core and Reactjs.</p>
<p>👯 I’m looking to collaborate on Frontend developers on Reactjs, Angular, or Vue.</p>
<p>📫 Reach me via https://t.me/air2921</p>

```cs
[HttpGet("{username}")]
public async Task<IActionResult> GetUser([FromRoute] string username)
{
    var userTask = _userRepository.GetByFilter(query => query.Where(u => u.username.Equals(username)));

    var myStack = new
    {
        languages = new string[] { "C#", "linq", "TypeScript" },
        tools = new string[] { "RESTApi/JSONApi", "Swagger", "Postman", "SignalR" },
        frameworks = new
        {
            backend = new string[] { "ASP.NET Core Web API", "ASP.NET Core MVC" },
            frontend = new string[] { "React.js", "html5", "css3" }
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
}
```
