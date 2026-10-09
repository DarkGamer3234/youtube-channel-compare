# Channel Clash — YouTube Channel Compare

A responsive GitHub Pages website for comparing two YouTube channels. It is configured for `@dubbet` and `@flamifytv` by default; you can change the handles in **API settings**.

## Features
- Subscriber counts, channel views, and public video counts
- Latest public upload with thumbnail, date, and views when available
- Combined totals and subscriber comparison bars
- Mobile-friendly dark design with orange accents
- API key stored in the browser's local storage

## Publish on GitHub Pages
1. Upload `index.html` and `README.md` to the root of your GitHub repository.
2. In the repository, open **Settings → Pages**.
3. Under **Build and deployment**, select **Deploy from a branch**.
4. Select your main branch and `/(root)`, then save.
5. Open the GitHub Pages URL shown on that page.

## Set up the YouTube API
1. Open [Google Cloud Console](https://console.cloud.google.com/).
2. Create or select a project.
3. Enable **YouTube Data API v3**.
4. Create an API key under **APIs & Services → Credentials**.
5. Open the site, click **API settings**, and paste the key.

For a public site, restrict the key to YouTube Data API v3 and configure website referrer restrictions where practical. Browser-side keys can be seen by visitors, so protect the key and monitor API quota.

## Notes
- Uses YouTube's official Data API; quota limits apply.
- Subscriber counts may be rounded or hidden by YouTube.
- Only public information available to the API key is shown.
- No backend is used; the key is saved in the browser that entered it.
