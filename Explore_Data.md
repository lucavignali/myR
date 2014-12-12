---
title: "Explore Data"
author: "Luca Vignali"
date: "Tuesday, December 09, 2014"
output: html_document
---


### Numeric Exploration 
* str()
* summary(numeric)
* head()
* table(factor)
* quantile(numeric, probs) / median(numeric)


### Base Plot System
#### Parameters
* pch
* lty
* lwd
* col / colors()
* xlab
* ylab
* par() / las, bg, mar, oma, mfrow, mfcol
* example(points)
* demo("graphics")
* type ="n"

#### Functions to adjust graphics
* lines
* points()
* text
* title
* mtext
* axis
* legend

#### Functions to create graphics
* plot
* boxplot
* hist
* Devices / windows(), pdf(), png(), .... / dev.cur, dev.set, dev.copy. dev.copy2pdf, dev.off

#### One Variable
* boxplot(numeric, col, breaks, main)
* hist(numeric, col, main, subset) / rug(numeric)
* abline(v/h, lwd, col, lty)
* barplot(vector/matrix) for category.

#### Multiple Variables
* plot()
* boxplot(x~y, data, col, xlab, ylab)
* par(mfrow, mar, new)
* with(subset, {plot(,,col), points(), type....})

### Lattice Plot System - libriaries lattice and grid
* xyplot(y ~ x | a * b, data, layout)
* bwplot
* histograms
* dotplot
* splom
* levelplot, contourplot
* print
* panel
* trellis.par.set

### ggplot2
* qplot (x,y,data, color, geom (smooth, density, point), facets ., fill, shape, method, binwidth)
* '+'
* ggplot (dataframe, aes) / summary
* '+'
* geom_point(color, size, alpha, aes()) 
* geom_somooth(method, size, linetype, se )
* facet_grid(.~.)
* facet_wrap
* xlab(), ylab(), labs(title,), ggtitle()
* theme(), theme_gray(), theme_bw(base_family = , base_size)
* ylim
* coord_cartesian()
