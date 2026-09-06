# Saksham-social-studies
Social studies material
from pathlib import Path

path = Path("/mnt/data/class10_social_science_website.html")
html = path.read_text(encoding="utf-8")
html = html.replace("Class 10 Social Science Hub", "Saksham Social Studies")
html = html.replace("SST<span>10</span> • Study Hub", "Saksham <span>Social Studies</span>")
html = html.replace("Made for Class 10 Social Science • Learn • Revise • Practice",
                    "Saksham Social Studies • Class 10 • Learn • Revise • Practice")
path.write_text(html, encoding="utf-8")
print(f"Updated: {path}")
