# tester
Information technology
# List of words/phrases that explicitly give permission
permission_words = [
    "allow", "permit", "authorize", "consent", "approve", "agree", "accept",
    "endorse", "grant", "sanction", "empower", "license", "give permission",
    "you may", "i consent", "i approve", "i agree", "i accept", "i grant"
]

# Example input (you could replace this with user input, file text, etc.)
text = input("Enter a sentence: ").lower()

# Check for explicit consent
found_permission = False
for word in permission_words:
    if word in text:
        print(f"✅ Explicit permission detected: '{word}'")
        found_permission = True
        break

if found_permission:
    print("Action is explicitly authorized.")
else:
    print("❌ No explicit permission detected. Action not authorized.")
