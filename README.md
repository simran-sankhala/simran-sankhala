### Hi there 👋

![profile picture](https://i.giphy.com/media/jrnlTtQdMwdpzXs1l7/giphy.webp)

- 🔭 I’m currently working as a Security Engineer
- 📫 How to reach me: https://simransankhala.surge.sh
- 😄 Pronouns: She/Her


```golang
package main

import (
	"os"
	"text/template"
)

type Bio struct {
	Name string
	Experience string
	Specialization string
	Certifications string
}

func main() {
	bio := Bio{
		Name: "Simran Sankhala",
		Experience: "3+ years of experience",
		Specialization: "Penetration Testing & Red Teaming",
		Certifications: "OSCP, CRTP, CTIA",
	}
	tmpl, err := template.New("bio").Parse(`My name is {{.Name}}, a Security Engineer with {{.Experience}}. Specializing in {{.Specialization}}. Having Certifications - {{.Cetifications}}.`)
	if err != nil {
		fmt.Println(err)
		os.Exit(1)
	}
	err = tmpl.Execute(os.Stdout, bio)
	if err != nil {
		fmt.Println(err)
		os.Exit(1)
	}
}
```

