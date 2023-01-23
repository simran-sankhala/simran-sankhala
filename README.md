### Hi I'm Simran  👋

![profile picture](https://media.tenor.com/Bpv9wTLKMskAAAAM/computer-nerds.gif)

- 🔭 I’m currently working as a Security Engineer



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

