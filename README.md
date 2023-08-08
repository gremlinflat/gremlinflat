### Hi there 👋

<!--
Hey guys, thank you for visiting these raw docs, (pls don't steal it, I've worked hard writing it. haha jk 🥲)
-->

```cpp
// Profile.cpp

#include "Skill.h" 
#include <vector>

class Profile {
private:
    std::string name;
    std::string username;
    std::string about;
    std::vector<Skill::TechStack> stacks;

public:
    Profile(const std::string& n, const std::string& u, const std::string& a);

    void addStacks(const Skill::TechStack& stacks);
    void flex();
};

int main() {
    Profile literallyMe("Fahri Novald", "gremlinflat", "I talk to machine");

    // Adding skills using TechStack namespace along with years of experience
    literallyMe.addSkill(Skill::TechStack::CPP(5));
    literallyMe.addSkill(Skill::TechStack::Python(10));
    literallyMe.addSkill(Skill::TechStack::Javascript(3));
    literallyMe.addSkill(Skill::TechStack::Swift(2));
    literallyMe.addSkill(Skill::TechStack::Dart(2));

    literallyMe.flex();

    return 0;
}


```
