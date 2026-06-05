import pandas as pd

# 1. Read your local CSV file
df = pd.read_csv('Appendix - Table1.csv')

# 2. Convert it to Markdown table format
markdown_table = df.to_markdown(index=False)

# 3. Print the code to copy-paste or write directly to a README
print(markdown_table)

# Optional: Save it directly into your README file
with open("README.md", "a") as f:
    f.write("\n### Table 1\n")
    f.write(markdown_table)
