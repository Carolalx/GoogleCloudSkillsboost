# Build an AI-Powered Interview Question Generator using Gemini

1 - Clique em File > New File para abrir um novo arquivo com o Editor de Código.   
2 - Copie e código abaixo e cole no Editor.   

```bash

import vertexai
from vertexai.generative_models import GenerativeModel

def interview(prompt):
    vertexai.init()
    model = GenerativeModel("gemini-2.5-flash-lite")
    response = model.generate_content(prompt)
    return response.text

# Custom prompt example
if __name__ == "__main__":
    custom_prompt = input("Enter your prompt: ") or "Give me ten interview questions for the role of program manager."
    result = interview(custom_prompt)
    print("\n" + "="*50)
    print(result)
    print("="*50)

```
3 - CLique em File > Save. Nomeie o Arquivo exatamente conforme o solicitado pelo LAB, ex.: FILE_NAME.py    
4 - Execute o arquivo Python com o comando informado no LAB    
```/usr/bin/python3 /FILE_NAME.py```

5 - Quando o terminal solicitar "Enter with your prompt" digite:   
```interview(prompt)```

---
6 - Pressione ENTER, aguarde alguns segundos e verifique seu progresso.
