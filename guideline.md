## 🕷️ Crawljax CLI Usage Guide

### 🛠️ Setup Instructions

1. **Clone the repository** (if not already):

   ```bash
   git clone <repo-url>
   cd <repo-folder>
   ```

2. **Apply Spotless formatting** (from the root folder):

   ```bash
   mvn spotless:apply
   ```

3. **Build the project (skip tests)**:

   ```bash
   mvn clean install -DskipTests
   ```

---

### 🐚 CLI Usage

4. **Navigate to the CLI module folder**:

   ```bash
   cd cli
   ```

5. **Fix JAR signature issue (run from inside `cli`):**

   ```bash
   zip -d target/crawljax-cli-5.2.4-SNAPSHOT.jar META-INF/*.RSA META-INF/*.SF
   ```

6. **Run Crawljax CLI**:

   ```bash
   java -jar target/crawljax-cli-5.2.4-SNAPSHOT.jar http://127.0.0.1:4000 ./outputfolder
   ```

---

### 📁 Output

* The crawled results will be saved in the `./outputfolder`.

---

