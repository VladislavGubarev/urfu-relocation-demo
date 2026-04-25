# Upload files

Upload these files to the same public HTTPS directory:

- `index.html`
- `urfu-relocation-demo.apk`

Recommended public URL:

`https://YOUR_DOMAIN_OR_PATH/index.html`

Recommended server MIME type for APK:

`application/vnd.android.package-archive`

Nginx example:

```nginx
types {
    application/vnd.android.package-archive apk;
}
```

Android will still show the normal "install from unknown source" prompt for APKs outside Google Play.
