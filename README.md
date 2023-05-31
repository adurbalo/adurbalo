```swift
let contactInformation = ContactInformation(email: "andrii.durbalo@gmail.com",
                                            phone: "+31 6 57 66 15 07",
                                            linkedIn: "http://www.linkedin.com/in/adurbalo",
                                            github: "https://github.com/adurbalo")

let skills = Skills(programmingLanguages: ["Swift",
                                           "Objective-C"],
                    platforms: ["iOS"],
                    architectures: ["MVC",
                                    "MVP+C",
                                    "MVVM"],
                    scripting: ["Bash", "Ruby", "Python"], // mostly for automatization purposes
                    other: ["CI / CD (GitLab, Jenkins, GitHub Actions, Fastlane)",
                            "Dependency managers (CocoaPods, SwiftPM)",
                            "Project modularization",
                            "Shared components development",
                            "Release and provisioning activities",
                            "Internal and external interviewing",
                            "Design patterns",
                            "Troubleshooter"])

let me = SoftwareEngineer(firstName: "Andrii",
                          lastName: "Durbalo",
                          role: "iOS Software Engineer",
                          contactInformation: contactInformation,
                          skills: skills,
                          location: "Amsterdam, Netherlands 🇳🇱",
                          funFact: "Big fan of Dynamo Kyiv and Golden State Warriors, prefer electronic music like drum & bass or so.")

print("Hi there, my name is \(me.firstName). I'm a \(me.role). Nice to see you here 😉")

//MARK: - TL;DR

struct SoftwareEngineer {
    let firstName: String
    let lastName: String
    let role: String
    let contactInformation: ContactInformation
    let skills: Skills
    let location: String
    let funFact: String
}

struct ContactInformation {
    let email: String
    let phone: String
    let linkedIn: URL
    let github: URL
}

struct Skills {
    let programmingLanguages: [String]
    let platforms: [String]
    let architectures: [String]
    let scripting: [String]
    let other: [String]
}

extension URL: ExpressibleByStringLiteral {
    public init(stringLiteral value: String) {
        self = URL(string: value)!
    }
}
```
