![[probeklausur_aufgabe.pdf]]
-- -
# Aufgabe 1 (Mengenoperationen)
Gegeben seien die Mengen A={a,b,3,4} und B={1,2,a,b}.
1. Bestimmen sie $A\cap B$
2. Bestimmen sie $A \cup B$
3. Bestimmen sie $A\textbackslash B$
4. Bestimmen sie $\mathcal{P}(A\cap B)$

Lösung:
1. $\{a,b,3,4\} \cap \{1,2,a,b\} = \{a,b\}$
2. $\{a,b,3,4\} \cup \{1,2,a,b\} = \{a,b,3,4,1,2\}$
3. $\{a,b,3,4\} \textbackslash \{1,2,a,b\} = \{3,4\}$
4. $\mathcal{P}(\{a,b,3,4\} \cap \{1,2,a,b\}) = \mathcal{P}(\{a,b\}) = \{\emptyset, \{a\}, \{b\}, \{a,b\}  \}$

-- -
# Aufgabe 2 (Überlegungen mit Mengen)
Die beiden folgenden Aussagen gelten nicht allgemein für alle Mengen 𝐴, 𝐵, 𝐶. Finden Sie Gegenbeispiele für Mengen 𝐴, 𝐵, 𝐶 zu folgenden Aussagen:
1. $A \subseteq B \Rightarrow A \cap B \neq \emptyset$
2. $A \cap B \neq \emptyset \land B \cap C \neq \emptyset \Rightarrow A \cap C \neq \emptyset$

Lösung:
1.  sei $A = \emptyset$ und $B = \{1,2\}$
   dann ist
   $$\begin{align*}
   A \subseteq B &\Rightarrow A \cap B \neq \emptyset \\
   \emptyset \subseteq \{1,2\} &\Rightarrow \emptyset \cap \{1,2\} \neq \emptyset \\
   \top &\Rightarrow \emptyset \neq \emptyset\\
   \top &\Rightarrow \bot\\
   \end{align*}
   $$
   was die def. vom $\Rightarrow$ widerlegt
   somit ist die Aussage $A \subseteq B \Rightarrow A \cap B \neq \emptyset$ widerlegt.
<br>
1.  sei $A=\{1\}$, $B=\{1,2\}$ und $C=\{2\}$
   $$
   \begin{align*}
   A \cap B \neq \emptyset &\land B \cap C \neq \emptyset &&\Rightarrow A \cap C \neq \emptyset \\
   \{1\} \cap \{1,2\} \neq \emptyset &\land \{1,2\} \cap \{2\} \neq \emptyset &&\Rightarrow \{1\} \cap \{2\} \neq \emptyset\\
   \{1\}\neq \emptyset  &\land \{2\} \neq \emptyset &&\Rightarrow \emptyset \neq \emptyset \\
   \top &\land \top && \Rightarrow \bot \\
   \top &&&\Rightarrow \bot
   \end{align*}
   $$
   $$\top \Rightarrow \bot$$
   was die def. vom $\Rightarrow$ widerlegt
   somit ist die Aussage $A \cap B \neq \emptyset \land B \cap C \neq \emptyset \Rightarrow A \cap C \neq \emptyset$ widerlegt.
   
-- -
# Aufgabe 3 (Mengenbeweis)
Seien 𝑀, 𝑁 Mengen. Zeigen Sie, dass folgendes gilt:
1. $\mathcal{P}(M) \cap \mathcal{P}(N) \subseteq \mathcal{P}(M \cap N)$