# Welcome to SF_SITE

где располагается репозиторий с кодом, как посмотреть существующий код;
как устроен процесс внесения своих изменений в основную кодовую базу;
каковы правила именования веток;
как настроить свою среду разработки, требуется прикрепить ссылку на лежащий в проекте конфиг;
инструкция для младших сотрудников по слиянию веток, какие команды надо выполнить, чтобы:

## Description

🚀copy project /--/ git@github.com:EvgenyKut/image-search-application.git

Happy hacking!

## 📌 Process

The template for a full branch naming looks like this - `type/task-number-Jira_task-name`.

###### Types

The following abbreviations are used for types:

- `task` - development
- `spike` - spike, learning a new library. Anything that won't go into production
- `fix` - bug fixing
- `backup` - archiving old branches
- `relise` - release branch, grouping all tasks for a release

###### Jira Task Number

For example - LK-1009

###### Task Name

Arbitrary name added to facilitate orientation in branches

###### Final Example

`doc/LK-1009__tech-doc`

## 📌 VSCODE

To use the same Prettier rules in Visual Studio Code and share them across projects, you can add the Prettier configuration to your global user settings. Here's a step-by-step guide:

Open Visual Studio Code.

Press Shift + Command + P on macOS (or Shift + Ctrl + P on Windows/Linux) to open the command palette.

Type and select Preferences: Open Settings (JSON).

## 📌 GIT-Helper

# Creating Your Branch:

git checkout -b feature/my-feature

# Making Changes in Your Branch:

git add .
git commit -m "Description of your changes"

# Merging Changes with the Main Codebase:

git checkout main
git pull origin main
git checkout feature/my-feature
git merge main
git add .
git commit -m "Merge changes from main into feature/my-feature"
git push origin feature/my-feature
