# tableView

```swift 
func tableView(_ tableView: UITableView, commit editingStyle: UITableViewCellEditingStyle, forRowAt indexPath: IndexPath) {
  if editingStyle == .delete {
    print("Deleted")

    self.catNames.remove(at: indexPath.row)
    self.tableView.deleteRows(at: [indexPath], with: .automatic)
  }
}
