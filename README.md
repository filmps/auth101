# auth101

1. dotnet new webapp --auth Individual -o WebApp1
2. add service in program.cs
and
app.UseRouting();

app.UseAuthentication();
app.UseAuthorization();

3. dotnet add package Microsoft.VisualStudio.Web.CodeGeneration.Design
4. dotnet tool install --global dotnet-aspnet-codegenerator
5. dotnet aspnet-codegenerator identity -dc WebApp1.Data.ApplicationDbContext --files "Account.Register;Account.Login;Account.Logout;Account.RegisterConfirmation" –dbProvider sqlite
(or --useSqLite)

