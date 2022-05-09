```php
$tb=new Person(
  name: "Tolga Bektaş",
  email: "tolgabektas00@gmail.com",
  age: 22
);

$tb->setStatus(new Life\Status(
    interested: ["Laravel", "Flutter", "Unity2D", "Unity3D"],
    abilities:    [
      "To research and solve problems in a logical and consequential way without memorizing the code",
      "Good at reading and understanding code",
      "Hardworker",
      "Quick learner",
      "Solution oriented"
    ],
    hobbies: ["Cycling", "Walking with music", "Watching series and movies", "Reading books"]
));

$mySkills=new Life\Skills(
  languages: ["PHP", "Html/CSS", "JavaScript", "C#"],
  editors: ["VSCode", "Sublime Text"],
  frameworks: ["Laravel" , "Bootstrap", "Jquery", "Ajax"]
));

$dev = new Profession\Developer(person: $tb, skills: $mySkills);

while($dev->awake())  
{
  $dev->code();
}
```
