image-processing-tool/
├── prisma/
│ ├── schema.prisma
│ ├── migrations/
│ │ └── 001_init/
│ │ └── migration.sql
│ └── seed.ts
├── src/
│ ├── app/
│ │ ├── (auth)/
│ │ │ ├── signin/
│ │ │ │ └── page.tsx
│ │ │ ├── signup/
│ │ │ │ └── page.tsx
│ │ │ └── forgot-password/
│ │ │ └── page.tsx
│ │ ├── admin/
│ │ │ ├── layout.tsx
│ │ │ ├── page.tsx
│ │ │ ├── users/
│ │ │ │ └── page.tsx
│ │ │ └── analytics/
│ │ │ └── page.tsx
│ │ ├── api/
│ │ │ ├── admin/
│ │ │ │ ├── stats/
│ │ │ │ │ └── route.ts
│ │ │ │ └── users/
│ │ │ │ └── route.ts
│ │ │ ├── auth/
│ │ │ │ └── [...nextauth]/
│ │ │ │ └── route.ts
│ │ │ ├── health/
│ │ │ │ └── route.ts
│ │ │ ├── images/
│ │ │ │ ├── upload/
│ │ │ │ │ └── route.ts
│ │ │ │ ├── process/
│ │ │ │ │ └── route.ts
│ │ │ │ ├── download/
│ │ │ │ │ └── [id]/
│ │ │ │ │ └── route.ts
│ │ │ │ ├── metadata/
│ │ │ │ │ └── [id]/
│ │ │ │ │ └── route.ts
│ │ │ │ ├── crop/
│ │ │ │ │ └── route.ts
│ │ │ │ ├── compress/
│ │ │ │ │ └── route.ts
│ │ │ │ ├── convert/
│ │ │ │ │ └── route.ts
│ │ │ │ ├── palette/
│ │ │ │ │ └── route.ts
│ │ │ │ └── upscale/
│ │ │ │ └── route.ts
│ │ │ ├── user/
│ │ │ │ ├── profile/
│ │ │ │ │ └── route.ts
│ │ │ │ └── history/
│ │ │ │ └── route.ts
│ │ ├── dashboard/
│ │ │ ├── layout.tsx
│ │ │ ├── page.tsx
│ │ │ ├── history/
│ │ │ │ └── page.tsx
│ │ │ └── settings/
│ │ │ └── page.tsx
│ │ ├── tools/
│ │ │ ├── layout.tsx
│ │ │ ├── crop/
│ │ │ │ └── page.tsx
│ │ │ ├── compress/
│ │ │ │ └── page.tsx
│ │ │ ├── convert/
│ │ │ │ └── page.tsx
│ │ │ ├── palette/
│ │ │ │ └── page.tsx
│ │ │ ├── metadata/
│ │ │ │ └── page.tsx
│ │ │ └── upscale/
│ │ │ └── page.tsx
│ │ ├── about/
│ │ │ └── page.tsx
│ │ ├── globals.css
│ │ ├── layout.tsx
│ │ ├── page.tsx
│ │ ├── loading.tsx
│ │ ├── error.tsx
│ │ └── not-found.tsx
│ ├── components/
│ │ ├── ui/
│ │ │ ├── button.tsx
│ │ │ ├── input.tsx
│ │ │ ├── card.tsx
│ │ │ ├── dialog.tsx
│ │ │ ├── dropdown-menu.tsx
│ │ │ ├── progress.tsx
│ │ │ ├── slider.tsx
│ │ │ ├── tabs.tsx
│ │ │ ├── toast.tsx
│ │ │ ├── tooltip.tsx
│ │ │ └── index.ts
│ │ ├── common/
│ │ │ ├── Header.tsx
│ │ │ ├── Footer.tsx
│ │ │ ├── Navigation.tsx
│ │ │ ├── LoadingSpinner.tsx
│ │ │ ├── ErrorBoundary.tsx
│ │ │ └── ThemeProvider.tsx
│ │ ├── auth/
│ │ │ ├── SignInForm.tsx
│ │ │ ├── SignUpForm.tsx
│ │ │ ├── AuthProvider.tsx
│ │ │ └── ProtectedRoute.tsx
│ │ ├── image/
│ │ │ ├── ImageUploader.tsx
│ │ │ ├── ImagePreview.tsx
│ │ │ ├── ImageGallery.tsx
│ │ │ ├── ImageCanvas.tsx
│ │ │ └── ImageMetadata.tsx
│ │ ├── tools/
│ │ │ ├── CropTool.tsx
│ │ │ ├── CompressTool.tsx
│ │ │ ├── ConvertTool.tsx
│ │ │ ├── PaletteTool.tsx
│ │ │ ├── MetadataTool.tsx
│ │ │ └── UpscaleTool.tsx
│ │ ├── dashboard/
│ │ │ ├── DashboardLayout.tsx
│ │ │ ├── StatsCard.tsx
│ │ │ ├── RecentActivity.tsx
│ │ │ └── QuickActions.tsx
│ │ └── admin/
│ │ ├── AdminLayout.tsx
│ │ ├── UserManagement.tsx
│ │ ├── SystemStats.tsx
│ │ └── Analytics.tsx
│ ├── lib/
│ │ ├── auth.ts
│ │ ├── db.ts
│ │ ├── storage.ts
│ │ ├── redis.ts
│ │ ├── queue.ts
│ │ ├── utils.ts
│ │ ├── constants.ts
│ │ ├── validations.ts
│ │ ├── image-processing/
│ │ │ ├── sharp-processor.ts
│ │ │ ├── canvas-processor.ts
│ │ │ ├── metadata-extractor.ts
│ │ │ ├── color-palette.ts
│ │ │ ├── compression.ts
│ │ │ ├── format-converter.ts
│ │ │ ├── cropper.ts
│ │ │ └── upscaler.ts
│ │ └── services/
│ │ ├── image-service.ts
│ │ ├── user-service.ts
│ │ ├── storage-service.ts
│ │ ├── analytics-service.ts
│ │ └── notification-service.ts
│ ├── hooks/
│ │ ├── useAuth.ts
│ │ ├── useImageProcessing.ts
│ │ ├── useUpload.ts
│ │ ├── useLocalStorage.ts
│ │ ├── useDebounce.ts
│ │ └── useToast.ts
│ ├── store/
│ │ ├── auth-store.ts
│ │ ├── image-store.ts
│ │ ├── ui-store.ts
│ │ └── settings-store.ts
│ ├── types/
│ │ ├── auth.ts
│ │ ├── image.ts
│ │ ├── user.ts
│ │ ├── api.ts
│ │ └── database.ts
│ └── middleware.ts
├── public/
│ ├── icons/
│ │ ├── icon-192x192.png
│ │ └── icon-512x512.png
│ ├── images/
│ │ ├── hero-bg.jpg
│ │ ├── placeholder.svg
│ │ └── logo.svg
│ ├── manifest.json
│ ├── robots.txt
│ └── favicon.ico
├── docs/
│ ├── API.md
│ ├── CONTRIBUTING.md
│ ├── DEPLOYMENT.md
│ └── DEVELOPMENT.md
├── scripts/
│ ├── build.sh
│ ├── deploy.sh
│ ├── seed-db.ts
│ └── backup-db.ts
├── .github/
│ ├── workflows/
│ │ ├── ci.yml
│ │ ├── cd.yml
│ │ └── tests.yml
│ ├── ISSUE_TEMPLATE/
│ │ ├── bug_report.md
│ │ └── feature_request.md
│ └── pull_request_template.md
├── README.md
├── LICENSE
├── package.json
├── .env
├── .env.local
├── .env.production
├── .gitignore
├── next.config.ts
├── postcss.config.js
├── tsconfig.json
├── docker-compose.yml
├── Dockerfile
