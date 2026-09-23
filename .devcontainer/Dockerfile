FROM ://microsoft.com

RUN apt-get update && apt-get install -y wget gnupg gnupg2 unzip \
    && wget -q -O - https://google.com | apt-key add - \
    && echo "deb [arch=amd64] http://google.com stable main" >> /etc/apt/sources.list.d/google-chrome.list \
    && apt-get update \
    && apt-get install -y google-chrome-stable \
    && apt-get clean && rm -rf /var/lib/apt/lists/*
