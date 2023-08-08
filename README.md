### Howdy 👋
![visitors](https://visitor-badge.laobi.icu/badge?page_id=gremlinflat.gremlinflat)

<!--
Well, well, look who's here peeking at my coding sanctuary! Feel free to take a gander, but remember, stealing's just so unoriginal (but hey, if you've got that urge, who am I to stop you? 🥱)
-->

```cpp
// Profile.cpp

#include <vector>
#include "Skill.h"
#include "Company.h"

class Profile {
private:
    std::string name;
    std::string username;
    std::string about;
    bool isOpenForOpportunity;
    Company::Workplace* workplace; 
    std::vector<Skill::TechStack> stacks;

public:
    Profile(const std::string& n, const std::string& u, const std::string& a);
    ~Profile(); // Destructor to clean up memory

    void addStacks(const Skill::TechStack& stacks);
    void flex();
    void unflex();
};

Profile::Profile(const std::string& n, const std::string& u, const std::string& a)
    : name(n), username(u), about(a), isOpenForOpportunity(false), workplace(nullptr) {}

Profile::~Profile() {
    delete workplace;
}

int main() {
    Profile literallyMe("Fahri Novald", "gremlinflat", "I talk to machines");

    // Stacks and years of experience.
    // Who needs frameworks? I code like a space cowboy, armed with a Vim and '90s Shinji's mixtape. No hug & kisses, just bug & fixes.
    literallyMe.addStack(Skill::TechStack::CPP(5)); 
    literallyMe.addStack(Skill::TechStack::Python(10));
    literallyMe.addStack(Skill::TechStack::Javascript(3));
    literallyMe.addStack(Skill::TechStack::Swift(2));
    literallyMe.addStack(Skill::TechStack::Dart(2));

    // Career
    literallyMe.isOpenForOpportunity = true; //🤧
    literallyMe.workplace = nullptr; // Unchained and ready to seize the bounty of opportunities, one code at a time! 💰🌟

    literallyMe.flex();

    return 0;
}

```

### 💀 Ping me a beacon!:
- 📧 Email: fnovaldi@icloud.com
- 📝 Medium: [medium.com/@gremlinflat](https://medium.com/@gremlinflat)
- ❌ ~~Twitter~~: [@gremlinflat_](https://twitter.com/gremlinflat_)

