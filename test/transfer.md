```
# Stop SpiderFoot first (Ctrl+C)

# Delete Python cache files
find /home/user/spiderfoot -type d -name "__pycache__" -exec rm -rf {} + 2>/dev/null
find /home/user/spiderfoot -name "*.pyc" -delete 2>/dev/null

# Pull latest changes
cd /home/user/spiderfoot
git pull

# Restart SpiderFoot
python3 ./sf.py -l 127.0.0.1:5001
```
