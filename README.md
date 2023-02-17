# MBPP: Mises Book PDF Project

A python script to scrape PDF books from the Mises Institute library website. Requires the Beautiful Soup library.

## How it works

1. Loads page at ```https://mises.org/library/books?book_type=539```
2. Scrapes each entry's author, title, post date, and download link
3. Downloads each entry's PDF file using ```YYYY-MM-DD_AuthorName_BookTitle.pdf``` naming convention
4. Loads next page

## Usage

Make the script executable and run at the command line.

To make sure you're downloading the entire library, first verify how many pages of pagination there are at the link above. As of February 2023 there were 57 pages, with the last URL located at ```https://mises.org/library/books?book_type=539&page=56```, so the script uses ```range(0, 56)``` in the forloop. Update this as needed.

## Support

You can support the Mises Institute by [donation](https://mises.org/giving/now) or [store](https://store.mises.org/).
