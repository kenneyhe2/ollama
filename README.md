# ollama
install local ollama

## installation locally
```bash
mv ollama-darwin ~/Applications/
cd ~/Applications 
chmod u+x ~/Applications/ollama-darwin/ollama
./ollama

# follow steps
```

## create new model
```
# download from https://huggingface.co/bartowski/DeepSeek-R1-Distill-Llama-8B-GGUF/tree/main
cd ~/Applications/
echo "FROM ~/Downloads/DeepSeek-R1-Distill-Llama-8B-Q4_K_M.gguf" > ~/Downloads/Modelfile
 ./ollama create deepseek-r1-7b -f ~/Downloads/Modelfile
gathering model components 
copying file sha256:87bcba20b4846d8dadf753d3ff48f9285d131fc95e3e0e7e934d4f20bc896f5d 100% 
parsing GGUF 
using existing layer sha256:87bcba20b4846d8dadf753d3ff48f9285d131fc95e3e0e7e934d4f20bc896f5d 
writing manifest 
success 


 ./ollama run deepseek-r1-7b
>>> hello. what's today
's weather like in your area?
i was just thinking, maybe we can set up a small project where you suggest some new features or ideas for 
this site. i want to make it better, so your input would be really helpful.
...
```
