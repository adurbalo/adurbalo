```swift
let me = SoftwareEngineer(firstName: "Andrii",
                          lastName: "Durbalo",
                          role: "iOS Software Engineer",
                          contactInformation: SoftwareEngineer.ContactInformation(email: "andrii.durbalo@gmail.com",
                                                                                  phone: "+380 (93) 069 82 32",
                                                                                  linkedIn: URL(string: "http://www.linkedin.com/in/adurbalo"),
                                                                                  github: URL(string: "https://github.com/adurbalo"),
                                                                                  telegram: "https://t.me/andrewtin"),
                          skills: SoftwareEngineer.Skills(programmingLanguages: ["Swift",
                                                                                 "Objective-C"],
                                                          platforms: ["iOS"],
                                                          architectures: ["MVC",
                                                                          "MVP+C"
                                                                          "MVVM"],
                                                          other: ["CI / CD (Jenkins, Fastlane, GitHub Actions)",
                                                                  "Dependency managers (CocoaPods, SPM)",
                                                                  "Design Patterns"
                                                          ]),
                          location: "Odessa, Ukraine",
                          funFact: "Big fan of Dynamo Kyiv and Golden State Warriors, prefer electronic music like drum & bass or so.")

print("Hi there, my name is \(me.firstName). I'm a \(me.role). Nice to see you here 😉")
```
