import React, { useEffect } from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { motion, useAnimation } from "framer-motion";

const techStack = [
  "Java", "Spring Boot", "React.js", "AWS", "Docker", "Kubernetes", "Kafka", "MongoDB",
  "Azure", "PostgreSQL", "Redux", "CI/CD", "OAuth2", "JWT"
];

const experiences = [
  {
    title: "Java Full Stack Developer",
    company: "NYC Health + Hospitals",
    duration: "May 2024 – Present",
    highlights: [
      "Developed HIPAA-compliant Patient Management Portal with Spring Boot & React.",
      "Migrated monolithic systems to Azure microservices with Kafka alerting.",
      "Built real-time messaging & appointment system using OAuth2 APIs."
    ]
  },
  {
    title: "Java Full Stack Developer",
    company: "Cognizant",
    duration: "Mar 2021 – Aug 2023",
    highlights: [
      "Built Member360 web app serving 8M+ users with AWS EKS & microservices.",
      "Implemented SSO, RBAC & secure APIs with JWT & OAuth2.",
      "Deployed CI/CD pipelines and migrated data pipelines to MongoDB/PostgreSQL."
    ]
  },
  {
    title: "Software Engineer",
    company: "Cred",
    duration: "Jan 2020 – Mar 2021",
    highlights: [
      "Developed reward redemption & credit payment gateway with React & Spring Boot.",
      "Built dashboards, transaction history APIs, and deployed services in Docker/ECS.",
      "Implemented microservices & test automation with 90%+ code coverage."
    ]
  }
];

const Portfolio = () => {
  const controls = useAnimation();

  useEffect(() => {
    const sequence = async () => {
      await controls.start({ opacity: 1, y: 0, transition: { duration: 1 } });
      await controls.start({ scale: 1.1, transition: { duration: 0.5 } });
      await controls.start({ scale: 1, transition: { duration: 0.5 } });
    };
    sequence();
  }, [controls]);

  return (
    <div className="min-h-screen bg-gradient-to-br from-purple-900 via-indigo-900 to-gray-900 text-white p-8">
      <motion.h1 
        className="text-5xl font-bold text-center mb-10 drop-shadow-xl"
        initial={{ opacity: 0, y: -50 }} 
        animate={controls}
      >
        Venkata Sai Sunil Bhattar Paruchuri
      </motion.h1>

      <motion.div
        className="flex flex-wrap justify-center gap-4 mb-12"
        initial="hidden"
        animate="visible"
        variants={{
          hidden: {},
          visible: {
            transition: {
              staggerChildren: 0.15
            }
          }
        }}
      >
        {techStack.map((tech, i) => (
          <motion.div
            key={i}
            initial={{ opacity: 0, y: -20 }}
            animate={{ opacity: 1, y: 0 }}
            transition={{ duration: 0.5, delay: i * 0.1 }}
            whileHover={{ scale: 1.2, rotate: 5 }}
            className="relative w-24 h-24 bg-gradient-to-br from-cyan-500 to-purple-600 text-white flex items-center justify-center rounded-full shadow-xl hover:shadow-2xl cursor-pointer"
          >
            <span className="text-center text-sm font-semibold px-2 text-white drop-shadow-md">
              {tech}
            </span>
          </motion.div>
        ))}
      </motion.div>

      <motion.p
        className="text-center max-w-3xl mx-auto mb-14 text-lg text-gray-300 leading-relaxed"
        initial={{ opacity: 0, y: 40 }}
        animate={{ opacity: 1, y: 0 }}
        transition={{ duration: 1.2, delay: techStack.length * 0.1 }}
      >
        Futuristic Full Stack Developer with 4+ years of hands-on experience in crafting scalable healthcare, fintech, and enterprise-grade applications. Proven excellence in building secure, high-performance systems using modern Java, Spring Boot, React.js, microservices, and cloud-native technologies.
      </motion.p>

      <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
        <Card className="bg-gradient-to-br from-purple-800/60 via-blue-800/30 to-transparent border border-purple-500/30 shadow-xl backdrop-blur-xl">
          <CardContent className="p-6">
            <h2 className="text-2xl font-semibold mb-4">👨‍💻 Experience</h2>
            <div className="space-y-6">
              {experiences.map((exp, idx) => (
                <motion.div
                  key={idx}
                  className="bg-gradient-to-br from-purple-700/30 via-blue-700/20 to-transparent p-4 rounded-2xl border border-purple-500/20 shadow-md backdrop-blur"
                  whileHover={{ scale: 1.02 }}
                >
                  <h3 className="text-xl font-semibold text-white mb-1">{exp.title} - <span className="text-purple-400">{exp.company}</span></h3>
                  <p className="text-sm text-gray-400 mb-2">{exp.duration}</p>
                  <ul className="list-disc ml-5 text-gray-300 space-y-1">
                    {exp.highlights.map((item, i) => (
                      <li key={i}>{item}</li>
                    ))}
                  </ul>
                </motion.div>
              ))}
            </div>
          </CardContent>
        </Card>

        <Card className="bg-gradient-to-br from-purple-800/60 via-blue-800/30 to-transparent border border-purple-500/30 shadow-xl backdrop-blur-xl">
          <CardContent className="p-6">
            <h2 className="text-2xl font-semibold mb-4">🎓 Education</h2>
            <div className="bg-gradient-to-r from-indigo-800/30 to-transparent p-4 rounded-2xl border border-indigo-500/20 shadow-md">
              <p className="text-gray-300">
                M.S. in Engineering Science (Data Science), University at Buffalo, NY<br />
                B.Tech in Engineering, PVP Siddhartha Institute of Technology, India
              </p>
            </div>
          </CardContent>
        </Card>

        <Card className="bg-gradient-to-br from-purple-800/60 via-blue-800/30 to-transparent border border-purple-500/30 shadow-xl backdrop-blur-xl">
          <CardContent className="p-6">
            <h2 className="text-2xl font-semibold mb-4">📫 Contact</h2>
            <div className="bg-gradient-to-r from-indigo-800/30 to-transparent p-4 rounded-2xl border border-indigo-500/20 shadow-md">
              <p className="text-gray-300">
                📧 vsaisunilbparuchuri@gmail.com<br />
                📞 +1 716-970-8737
              </p>
              <Button className="mt-4 w-full" variant="secondary">Download Resume</Button>
            </div>
          </CardContent>
        </Card>
      </div>

      <footer className="mt-10 text-center text-gray-500 text-sm">
        ⚡ Built with React, TailwindCSS & Framer Motion · Deployed on futuristic dreams ⚡
      </footer>
    </div>
  );
};

export default Portfolio;
