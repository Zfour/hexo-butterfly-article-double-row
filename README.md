# hexo-butterfly-article-double-row
Change the layout of the hexo-theme-butterfly article to double columns

```css
#recent-posts{
	margin-top:-1rem;  /*头部为空时抵消间隔*/
	align-content:flex-start;
	display: flex;
    flex-wrap: wrap; /*规定灵活的项目在必要的时候拆行或拆列。*/
    justify-content: space-between; /*。*/
}
#recent-posts > .recent-post-item {
  /*max-height:324px;*/  /*文章容器最大高度*/
  margin-top: 1rem; /*最小间距*/
  display: inline-block;
  height:auto; /*高度自动*/
  width:49%;/*文章容器容器宽度*/
}
#recent-posts > .recent-post-item .post_cover {
  width: 100%; /*图片封面宽度*/
    height: 200px;/*图片封面高度*/
}
#recent-posts > .recent-post-item .post_cover img.post_bg {
  width: 100%;/*图片宽度*/
  height: 100%;/*图片高度*/
}


#recent-posts > .recent-post-item >.recent-post-info > .content {
display:none;/*隐藏文章详情*/
}
#recent-posts > .recent-post-item {

  -webkit-flex-direction: column; /*容器内部纵向排列*/
  -ms-flex-direction: column; /*容器内部纵向排列*/
  flex-direction: column; /*容器内部纵向排列*/

}
#recent-posts > .recent-post-item .left_radius {
    border-radius: 8px 8px 0 0;/*圆角修改*/
}
#recent-posts > .recent-post-item .right_radius {
    border-radius: 8px 8px 0 0;/*圆角修改*/
}
.recent-post-item{
	height:auto !important;/*容器高度自动*/
}

.recent-post-info {
  
  padding: 0 40px;/*容器内部文字左右间距*/
  margin-top: 1em;/*容器内部文字上间距*/
  width: 100%!important;/*容器宽度*/
}
#recent-posts > .recent-post-item > .recent-post-info > .article-title {
    -webkit-line-clamp: 1;/*控制标题的行数*/
    margin-top: 0.3rem; /*控制标题的上间距*/
	margin-bottom: 0.3rem;/*控制标题的下间距*/
    color: var(--text-highlight-color);
    font-size: 1.2em; /*控制标题的字体大小*/
    line-height: 1.4;/*控制标题的行高*/
 
}
#recent-posts > .recent-post-item >.recent-post-info > .article-meta-wrap {
	margin-bottom: 1rem;/*控制标题meta信息的底部间距*/
}
@media screen and (max-width: 768px) {
#recent-posts > .recent-post-item {
 width:100%;/*控制手机自适应*/
}


```
