# DataAnalysisMethods -INF506 TTurkish German University

ÜBUNG 1 invert normal_cdf by using binary search and plot data histogram (mu=0 and sigma=57)

ÜBUNG 2 Eine Münze wird 2, 3, 4, 5, 10, 15, 50, 150 Mal geworfen und jeder Wurf aufgezeichnet. Sie zeichnen und vergleichen die beobachteten posterioren Wahrscheinlichkeiten. (bitte kodieren Sie die Beta-Verteilung von Grund auf)

ÜBUNG 3

You should fetch the data from the URL http://spamassassin.apache.org/old/publiccorpus/ to create a spam filter dataset. This dataset should include emails annotated as spam (20030228_spam.tar.bz2) and not spam (20030228_easy_ham.tar.bz2)
print(len(ham_filenames)) print(len(spam_filenames))

After fetching, you should read and sort data in the folders. By using the parser api of the email package (https://docs.python.org/3/library/email.parser.html) you should be able to parse the content of the emails.
import email import email.policy print(ham_emails[1].get_content().strip()) print(spam_emails[6].get_content().strip())

Explore content type of emails whether they are text/plain or text/html. For plain text return content, otherwise return html to plain version.
X = np.array(spam_emails + ham_emails, dtype=object) sample_html_spam = X[0] print(html_to_plain_text(sample_html_spam.get_content()))

ÜBUNG 4 Iris-Dataset aus der sklearn-Bibliothek laden. (1) Datenverständnis; deskriptive Statistikergebnisse, Überprüfung von Nulleinträgen (2) Korrelationsanalyse (3) Ausreißeranalyse (4) explorative Datenanalyse; Plotten Sie paarweise Relationen von Features, Plotten Sie gemeinsame und marginale Verteilungen von zwei Features

Bitte kommentieren Sie alle Grafiken in den Spalten (2), (3), (4)
