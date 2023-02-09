### Hi I'm Simran  👋

![profile picture](https://media.tenor.com/Bpv9wTLKMskAAAAM/computer-nerds.gif)

- 🔭 I’m currently working as a Security Engineer



```css
┌[Simran☮git]-(~)
└> mefetch
```

<div style="display:block;text-align:left"><img align="left" src="https://user-images.githubusercontent.com/56447720/215329483-0f7dcda1-71a7-495a-9097-2393af297636.png" border="0" style="width:156px;">
  
  ```css
  Simra@GitHub
  -----------------
  Name: ["Simran Sankhala"],
  Experience: ["3+ years of experience"],
  Specialization: ["Penetration Testing & Red Teaming"],
  Certifications: ["OSCP, CRTP, CTIA"]
```



```golang
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

