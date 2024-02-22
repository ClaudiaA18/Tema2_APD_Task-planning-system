# Tema #2 APD - Planificarea de Task-uri Într-un Datacenter

## Student: Gîrniță Alexandra-Claudia
## Grupa: 332CC

### Descriere
Proiectul simulează planificarea eficientă a task-urilor într-un datacenter, implementând două clase principale în Java: `MyHost` și `MyDispatcher`. Această abordare vizează optimizarea procesului de alocare a resurselor și gestionarea task-urilor într-un mediu distribuit.

### Clase
#### 1. Clasa `MyHost`
Reprezintă un nod individual în sistemul de planificare, responsabil cu gestionarea și procesarea task-urilor folosind o coadă de priorități. Principalele sale metode includ:
- `run()`: Procesează task-urile așteptând și executându-le în ordinea priorității.
- `addTask(Task task)`: Adaugă un nou task în coada de priorități.
- `processCurrentTask()`: Simulează procesarea task-ului curent.
- `shutdown()`: Încheie prelucrarea task-urilor.

#### 2. Clasa `MyDispatcher`
Funcționează ca un dispatcher centralizat care distribuie task-uri către nodurile `MyHost` folosind diferite strategii:
- Round Robin (RR)
- Shortest Queue (SQ)
- Size Interval Task Assignment (SITA)
- Least Work Left (LWL)
