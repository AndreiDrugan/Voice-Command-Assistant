Voice Command Assistant
Un asistent local în Python care transcrie fișiere audio folosind OpenAI Whisper și mapează textul obținut la comenzi de sistem prin similaritate cosinus, pe baza unui set de date personalizat.

Cerințe preliminare
Înainte de a rula codul, asigurați-vă că aveți instalate următoarele dependențe pe sistem:

Python 3.10 sau o versiune ulterioară

FFmpeg (necesar pentru ca Whisper să poată decodifica fișierele audio și video)

Pentru a instala FFmpeg pe Windows, rulați în terminal:

Bash
winget install Gyan.FFmpeg
Instalare
Instalați pachetele necesare pentru Python rulând comanda:

Bash
pip install openai-whisper scikit-learn pandas numpy
Structura proiectului
main.ipynb - Notebook-ul principal care conține fluxul de transcriere, vectorizarea TF-IDF, calculul similitudinii cosinus și execuția comenzilor.

comenzi.csv - Setul de date cu frazele de referință și comenzile asociate.

Mod de utilizare
Asigurați-vă că aveți un fișier audio sau video (de exemplu, db.mp4) în directorul proiectului.

Deschideți fișierul Jupyter Notebook și rulați secvențial celulele pentru a încărca modelul Whisper, a procesa textul și a rula acțiunea corespunzătoare prin modurile subprocess sau webbrowser.
