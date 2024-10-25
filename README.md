    using System;

    class AboutMe 
    {

        // Personal Information
        string Name = "Anıl Yağız Başaran"; 
        string Role = "👨‍🎓 Computer Engineering Student & 💼 Freelancer"; 
        string Motto = "🌟 Building the future, one line of code at a time."; 
        string Website = "⏳ Coming Soon!"; 
        string Location = "📍 Istanbul";
    
        // Interests & Skills
        string[] Interests = { "🤖 AI", "📈 Machine Learning", "💻 Desktop Development" }; 
        string[] Skills = { "C#", "Python", "SQL", ".NET" };
    
        // Skill levels (0 to 100)
        int CSharpLevel = 90;
        int PythonLevel = 75;
        int SQLLevel = 80;
        int DotNetLevel = 85;
    
        // 📬 Contact Info
        string LinkedIn = "linkedin.com/in/anilyagizbasaran"; 
        string Email = "yagizzanil@gmail.com";
    
        // 🚀 Experience
        int YearsOfExperience = 5; 
        int FreelanceExperience = 2;
    
        // Entry point
        static void Main(string[] args) 
        {
            AboutMe aboutMe = new AboutMe();
            aboutMe.Code();
            aboutMe.DevelopWebsite();
        }
    
        void Code() 
        { 
            Console.WriteLine("Coding and freelancing from Istanbul 🌍"); 
            Console.WriteLine("🌟 " + Motto); 
            ShowSkillLevels(); // Display skill levels
        }
    
        // Method to show skill levels as progress bars
        void ShowSkillLevels() 
        {
            Console.WriteLine("\n🔧 Skill Levels:");
            DisplayProgressBar("C#", CSharpLevel);
            DisplayProgressBar("Python", PythonLevel);
            DisplayProgressBar("SQL", SQLLevel);
            DisplayProgressBar(".NET", DotNetLevel);
        }
    
        // Helper method to display a progress bar
        void DisplayProgressBar(string skill, int level) 
        {
            Console.Write(skill + ": ");
            int progressBarLength = 20; // Length of the progress bar
            int filledLength = (int)((level / 100.0) * progressBarLength);
            string progressBar = new string('█', filledLength) + new string('░', progressBarLength - filledLength);
            Console.WriteLine($"[{progressBar}] {level}%");
        }
    
        // Web Development method with a simplified loop 
        void DevelopWebsite() 
        { 
            string[] steps = { 
                "Planning the website... 📝", 
                "Designing the UI... 🎨", 
                "Coding the frontend... 💻", 
                "Setting up the backend... ⚙️", 
                "Testing and deploying... 🚀" 
            };
    
            foreach (var step in steps) 
            { 
                Console.WriteLine(step); 
            } 
        }  
    }
